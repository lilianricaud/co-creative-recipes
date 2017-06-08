---
ID: 1798
post_title: 'Towards a #GitWeb for distributed collaboration'
author: lilian
post_date: 2014-07-02 14:29:42
post_excerpt: ""
layout: post
permalink: >
  http://liric.dreamhosters.com/recipes/2014/07/02/towards-a-gitweb-for-distributed-collaboration/
published: true
embed_code:
  - ""
  - ""
  - ""
likes_count:
  - "2"
  - "2"
  - "2"
voted_IP:
  - 'a:2:{i:0;s:11:"194.6.220.9";i:1;s:13:"88.160.52.138";}'
  - 'a:2:{i:0;s:11:"194.6.220.9";i:1;s:13:"88.160.52.138";}'
  - 'a:2:{i:0;s:11:"194.6.220.9";i:1;s:13:"88.160.52.138";}'
---
<em>Git and github are great tools for <a title="Stigmergic Collaboration" href="http://www.co-creative-recipes.cc/stigmergic-collaboration/">distributed collaboration and stigmergy</a>. Could we apply the same principles to work collaborativelly <em>using our current existing platforms</em> yet collaborate in a permission-less, distributed manner  ?</em>
<h2>The current state of the web: CMS silos &amp; platforms overkill</h2>
In the field of <a href="http://www.lilianricaud.com/web-strategy/open-research/open-social-innovation-open-sourcing-social-innovation-to-promote-sharing-sustainable-social-practices/">Open Social Innovation</a> there are several great ressources but they all use a different CMS:
<ul>
	<li><a href="http://www.bretagne-creative.net/">Bretagne Creative</a> runs on <a href="http://www.spip.net/en_rubrique25.html">SPIP</a></li>
	<li><a href="http://movilab.org/">MoviLab</a> and <a href="https://en.wikipedia.org/">Wikipedia</a> run on <a href="https://www.mediawiki.org/">Mediawiki</a></li>
	<li><a href="http://www.lilianricaud.com/web-strategy/case-study-how-to-co-create-a-co-creative-event/">Outils Réseaux / MousTIC and the Archipel network</a> are using <a href="http://yeswiki.net/">YesWiki</a></li>
	<li><a href="http://co-creative-recipes.cc/">Co-Creative Recipes.cc</a> runs on <a href="http://wordpress.org/">Wordpress</a></li>
	<li><a href="http://imaginationforpeople.org/en/">Imagination for People</a> is using its own customs CMS</li>
</ul>
Although these projects are all using free licences and free/libre opens source CMS, in practice copying and modiying from each other is not straighforward and there is a silo effect.
<h2>The Git/GitHub model</h2>
Git/<a href="https://github.com/">GitHub</a> makes it super easy to make personal variants while keeping a way to share and reuse content between parallel projects (“Forks”). Linus Torvald (the creator of Git) has changed the social dynamic around forking, <strong>turning the idea of multiple versions of a work from a cultural weakness into a cultural strength</strong> (Read <a href="http://dashes.com/anil/2010/09/forking-is-a-feature.html">Forking is a Feature</a>).

Ideally everyone should be using Git/GitHub to share content so that it can be easily reused by everyone else. In practice however there are 2 majors issues:
<ul>
	<li>Git/GitHub is designed to work with code and although Github is more user friendly, it is still not obvious for the average publisher</li>
	<li>there isn't and there won't be any ideal platform that suits everyone and content producers will want to keep using their existing platform</li>
</ul>
Could we apply the Git/GitHub model to the web itself and make it easy to share content between existing platform ?

Here's a little scenario inspired by the <a href="http://indiewebcamp.com/">#indieweb</a> approach.
<h2>Imagine #GitWeb: User story</h2>
<em>Imagine</em>:

I'm on the wikipedia page for "hackathon" and I want to modify it for my own purpose. Because Wikipedia has become part of the Gitweb netwok, it feature a "fork me on GitWeb" ribbon.

&nbsp;

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wikipedia-gitweb.jpg"><img class="aligncenter size-large wp-image-1799" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wikipedia-gitweb-1024x664.jpg" alt="hackathon-wikipedia-gitweb" width="770" height="499" /></a>

When I clik on this button it will import the content (title, body content, #tags, link to the originl article...) in my Co-Crative recipes site where I will be able to modify the content locally in my own Wordpress install.

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-edition-mode-gitweb.jpg"><img class="aligncenter size-large wp-image-1800" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-edition-mode-gitweb-1024x729.jpg" alt="hackathon-edition-mode-gitweb" width="770" height="548" /></a>

I can add an image, text, ... make my own personal version of the content.

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-co-creative-recipes.jpg"><img class="aligncenter size-large wp-image-1801" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-co-creative-recipes-1024x596.jpg" alt="hackathon-co-creative-recipes" width="770" height="448" /></a>

When I save my new content, I can decide to do a "pull request", ie inform the original content creators that I made a new version and that they might want to update their own version by "pulling" my modifications into their page and CMS.

A versionning tool allow them to quickyl see what I have changed and decide which modifications they want to integrate.

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-mediawiki-versionning.jpg"><img class="aligncenter size-large wp-image-1803" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-mediawiki-versionning-1024x619.jpg" alt="hackathon-mediawiki-versionning" width="770" height="465" /></a>

Similarly if someone using SPIP, YesWiki or Drupal fork one of my page and save it, I get a ping/pull request telling me which page has been forked and modified and short summary of the changes.

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/wordpress-pingback-pull-request.jpg"><img class="aligncenter size-large wp-image-1804" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/wordpress-pingback-pull-request-1024x200.jpg" alt="wordpress-pingback-pull-request" width="770" height="150" /></a>

I can quickly visualize the changes using my own Wordpress versionning tool:

<a href="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wordpress-versionning.jpg"><img class="aligncenter size-large wp-image-1805" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wordpress-versionning-1024x686.jpg" alt="hackathon-wordpress-versionning" width="770" height="515" /></a>

Hee again I can choose to add the updates to my own branch or leave it as is.
<h2>Approach</h2>
Here are some ideas about the practical approach that could underpin this scenario. I'm not developper, so this might need tweaking.
<ul>
	<li>A #Gitweb network of participants should agree on standards for content to clone (title, body content, #tags, link to original content ...) and free licence.</li>
	<li>From this each CMS should devellop a plugin that allows the following functions:
<ul>
	<li>add a "fork me" button.</li>
	<li> serve XML content to vsisitor sclicking the "fork me" button.</li>
	<li>the users is asked where to import the content into (in my case Wordpress) and to give its credential before being authorized to post</li>
	<li>the content is imported in a draft post where the user can edit and customize before saving it</li>
	<li>after saving the user can ping back/request pulling to the original site</li>
	<li>the site gets a list of pingback and can choose to moderate them, compare versions and eventually pick up modifications it want to add into the original article</li>
	<li>the user who forked the original content gets a notified when one of his modifications has been added back.</li>
</ul>
</li>
	<li>some anti-spam measures are built into the system to make it easy to weed out irrelevant notifications</li>
</ul>
<h2>Potential applications</h2>
The aim is to overcome traditionnal <a href="http://www.co-creative-recipes.cc/stigmergic-collaboration/#wiki-limitations">Wikis Limitations</a> and silos, thinking more in terms of protocol instaed of reinventing another platform:
<ul>
	<li><a title="Stigmergic Collaboration" href="http://www.co-creative-recipes.cc/stigmergic-collaboration/">it would allow distributed stigmergic collaboration</a>: distributed and permission less. No consensus required. People do their own things, yet everyone can easily reuse others people and feed from each other ideas.</li>
	<li><a title="Stigmergic Collaboration" href="http://www.co-creative-recipes.cc/stigmergic-collaboration/">it would </a>allows several versions and <strong>non neutral</strong> point of views to co-exist: instead of having one true version of a topic (imagine a controversial topic such as religion or politics), a wikipedia using #GitWeb could have several "non-neutral" points of views co-existing in parrallel, offering several version of the truth and uses could choose to read from different angles. In this mode having different radical points of views could be a feature and not a bug.</li>
</ul>
&nbsp;
<h2>Message in the bottle</h2>
I'm not sure how feasible this is. I had the idea in my mind for long time and to my knowledge this seems easily feasible in terms of technics. Growing a network around the idea is another thing and I'm releasing the idea in the wild hoping other can improve it or build upon it. I'll update the article as new ideas come.