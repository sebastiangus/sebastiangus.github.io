---
Author: "Sebastian Gustavsson"
layout: "post"
title: "Open Graph, what is it? whats the use?"
section:
tags:
section:
tags:
link_box: true
beginner_href:
intermediate_href:
advanced_href:
trivia_href:
source_href: [["http://ogp.me/",Open Graph]]
wikipedia_href: [["https://en.wikipedia.org/wiki/Facebook_Platform#Open_Graph_protocol",Open Graph a part of the Facebook Platform]]
---

#What is Open Graph?
Open Graph is a protocol to let web page creators make their content more presentable for social platforms. You ad meta-tags to your pages to let platforms scan your site and present accoirding to the protocol.


##How I use OG
I use OG to extract data about Title, Description (excerpt - first paragraph, stripped from HTML code), page.url, section, tags and author.

    <meta property="og:title" content="{{page.title}}" />
    <meta property="og:description" content="{{page.excerpt | strip_html}}" />
    <meta property="og:article:url" content="{{page.url}}" />
    <meta property="og:article:section" content="{{page.section}}" />
    {% for item in page.tags %}
    <meta property="og:article:tag" content="{{item}}" />
    {% endfor %}
    <meta property="og:article:author" content="https://github.com/sebastiangus" />


