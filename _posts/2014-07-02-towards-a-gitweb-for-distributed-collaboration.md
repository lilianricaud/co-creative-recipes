---
ID: 1798
post_title: 'Towards a #GitWeb for distributed collaboration'
author: lilian
post_date: 2014-07-02 14:29:42
post_excerpt: ""
layout: post
permalink: >
  http://www.co-creative-recipes.cc/towards-a-gitweb-for-distributed-collaboration/
published: true
embed_code:
  - ""
likes_count:
  - "2"
voted_IP:
  - 'a:2:{i:0;s:11:"194.6.220.9";i:1;s:13:"88.160.52.138";}'
---
*Git and github are great tools for [distributed collaboration and stigmergy][1]. Could we apply the same principles to work collaborativelly *using our current existing platforms* yet collaborate in a permission-less, distributed manner  ?* 
## The current state of the web: CMS silos & platforms overkill In the field of 

[Open Social Innovation][2] there are several great ressources but they all use a different CMS: 
*   [Bretagne Creative][3] runs on [SPIP][4]
*   [MoviLab][5] and [Wikipedia][6] run on [Mediawiki][7]
*   [Outils Réseaux / MousTIC and the Archipel network][8] are using [YesWiki][9]
*   [Co-Creative Recipes.cc][10] runs on [Wordpress][11]
*   [Imagination for People][12] is using its own customs CMS Although these projects are all using free licences and free/libre opens source CMS, in practice copying and modiying from each other is not straighforward and there is a silo effect. 

## The Git/GitHub model Git/

[GitHub][13] makes it super easy to make personal variants while keeping a way to share and reuse content between parallel projects (“Forks”). Linus Torvald (the creator of Git) has changed the social dynamic around forking, **turning the idea of multiple versions of a work from a cultural weakness into a cultural strength** (Read [Forking is a Feature][14]). Ideally everyone should be using Git/GitHub to share content so that it can be easily reused by everyone else. In practice however there are 2 majors issues: 
*   Git/GitHub is designed to work with code and although Github is more user friendly, it is still not obvious for the average publisher
*   there isn't and there won't be any ideal platform that suits everyone and content producers will want to keep using their existing platform Could we apply the Git/GitHub model to the web itself and make it easy to share content between existing platform ? Here's a little scenario inspired by the 

[#indieweb][15] approach. 
## Imagine #GitWeb: User story

*Imagine*: I'm on the wikipedia page for "hackathon" and I want to modify it for my own purpose. Because Wikipedia has become part of the Gitweb netwok, it feature a "fork me on GitWeb" ribbon.   [<img class="aligncenter size-large wp-image-1799" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wikipedia-gitweb-1024x664.jpg" alt="hackathon-wikipedia-gitweb" width="770" height="499" />][16] When I clik on this button it will import the content (title, body content, #tags, link to the originl article...) in my Co-Crative recipes site where I will be able to modify the content locally in my own Wordpress install. [<img class="aligncenter size-large wp-image-1800" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-edition-mode-gitweb-1024x729.jpg" alt="hackathon-edition-mode-gitweb" width="770" height="548" />][17] I can add an image, text, ... make my own personal version of the content. [<img class="aligncenter size-large wp-image-1801" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-co-creative-recipes-1024x596.jpg" alt="hackathon-co-creative-recipes" width="770" height="448" />][18] When I save my new content, I can decide to do a "pull request", ie inform the original content creators that I made a new version and that they might want to update their own version by "pulling" my modifications into their page and CMS. A versionning tool allow them to quickyl see what I have changed and decide which modifications they want to integrate. [<img class="aligncenter size-large wp-image-1803" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-mediawiki-versionning-1024x619.jpg" alt="hackathon-mediawiki-versionning" width="770" height="465" />][19] Similarly if someone using SPIP, YesWiki or Drupal fork one of my page and save it, I get a ping/pull request telling me which page has been forked and modified and short summary of the changes. [<img class="aligncenter size-large wp-image-1804" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/wordpress-pingback-pull-request-1024x200.jpg" alt="wordpress-pingback-pull-request" width="770" height="150" />][20] I can quickly visualize the changes using my own Wordpress versionning tool: [<img class="aligncenter size-large wp-image-1805" src="http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wordpress-versionning-1024x686.jpg" alt="hackathon-wordpress-versionning" width="770" height="515" />][21] Hee again I can choose to add the updates to my own branch or leave it as is. 
## Approach Here are some ideas about the practical approach that could underpin this scenario. I'm not developper, so this might need tweaking. 

*   A #Gitweb network of participants should agree on standards for content to clone (title, body content, #tags, link to original content ...) and free licence.
*   From this each CMS should devellop a plugin that allows the following functions: 
    *   add a "fork me" button.
    *    serve XML content to vsisitor sclicking the "fork me" button.
    *   the users is asked where to import the content into (in my case Wordpress) and to give its credential before being authorized to post
    *   the content is imported in a draft post where the user can edit and customize before saving it
    *   after saving the user can ping back/request pulling to the original site
    *   the site gets a list of pingback and can choose to moderate them, compare versions and eventually pick up modifications it want to add into the original article
    *   the user who forked the original content gets a notified when one of his modifications has been added back.
*   some anti-spam measures are built into the system to make it easy to weed out irrelevant notifications

## Potential applications The aim is to overcome traditionnal 

[Wikis Limitations][22] and silos, thinking more in terms of protocol instaed of reinventing another platform: 
*   [it would allow distributed stigmergic collaboration][1]: distributed and permission less. No consensus required. People do their own things, yet everyone can easily reuse others people and feed from each other ideas.
*   [it would ][1]allows several versions and **non neutral** point of views to co-exist: instead of having one true version of a topic (imagine a controversial topic such as religion or politics), a wikipedia using #GitWeb could have several "non-neutral" points of views co-existing in parrallel, offering several version of the truth and uses could choose to read from different angles. In this mode having different radical points of views could be a feature and not a bug.   

## Message in the bottle I'm not sure how feasible this is. I had the idea in my mind for long time and to my knowledge this seems easily feasible in terms of technics. Growing a network around the idea is another thing and I'm releasing the idea in the wild hoping other can improve it or build upon it. I'll update the article as new ideas come.

 [1]: http://www.co-creative-recipes.cc/stigmergic-collaboration/ "Stigmergic Collaboration"
 [2]: http://www.lilianricaud.com/web-strategy/open-research/open-social-innovation-open-sourcing-social-innovation-to-promote-sharing-sustainable-social-practices/
 [3]: http://www.bretagne-creative.net/
 [4]: http://www.spip.net/en_rubrique25.html
 [5]: http://movilab.org/
 [6]: https://en.wikipedia.org/
 [7]: https://www.mediawiki.org/
 [8]: http://www.lilianricaud.com/web-strategy/case-study-how-to-co-create-a-co-creative-event/
 [9]: http://yeswiki.net/
 [10]: http://co-creative-recipes.cc/
 [11]: http://wordpress.org/
 [12]: http://imaginationforpeople.org/en/
 [13]: https://github.com/
 [14]: http://dashes.com/anil/2010/09/forking-is-a-feature.html
 [15]: http://indiewebcamp.com/
 [16]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wikipedia-gitweb.jpg
 [17]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-edition-mode-gitweb.jpg
 [18]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-co-creative-recipes.jpg
 [19]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-mediawiki-versionning.jpg
 [20]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/wordpress-pingback-pull-request.jpg
 [21]: http://www.co-creative-recipes.cc/wp-content/uploads/2014/07/hackathon-wordpress-versionning.jpg
 [22]: http://www.co-creative-recipes.cc/stigmergic-collaboration/#wiki-limitations