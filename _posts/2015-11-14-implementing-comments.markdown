---
Author: "Sebastian Gustavsson"
layout: "post"
title: "Implementing comments with disqus"
category: ""
tags: ""
link_box: boolean
beginner_href: [["https://help.disqus.com/customer/portal/articles/1104788-web-integration",Getting started],["https://help.disqus.com/customer/portal/articles/472097-universal-embed-code", Code to embed]]
intermediate_href: [["https://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables", Disqus configuration],["http://jekyllrb.com/docs/variables/",]]
trivia_href:
source_href:
advanced_href:
wikipedia_href: [["https://en.wikipedia.org/wiki/Blog_comment_hosting_service", Blog comment hosting service]]
---

#Blog comment hosting service
I choosed to implement Disqus as recommended, but Disqus is just one of many blog comment providers. Please read more in the linked wikipedia article about "Blog comment hosting service".

#Implementation
I choosed to implement the script embeded in the HTML of each site instead of linking in the script. I created a separate disqus.html in the Jekyll _includes-folder.
If you place the code in a separate html-file it's possible to use the liquid command { &#37; include disqus.html &#37; }

##Embeding Disqus script
Embeding disqus is a piece of cake, just copy-paste the code according to their [instructions](https://help.disqus.com/customer/portal/articles/472097-universal-embed-code) and you'll be up and
running in seconds.

##Configure the script
I have used the [Liquid-variables](http://jekyllrb.com/docs/variables/): &#123;&#123; page.url &#125;&#125; and &#123;&#123; page.id &#125;&#125; to configure the script. The configuration
is made to let disqus know what unique page the script is loaded to, so it can present the right comments to the right page.
