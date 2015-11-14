---
Author: Sebastian Gustavsson
layout: post
title:  "My thoughts about pre-compiled CSS"
categories:
tags:
link_box: true
beginner_href: [["http://sass-lang.com/guide",Sass Basics],["http://thesassway.com/beginner",Sass.com],["http://lesscss.org/",less - getting started]]
intermediate_href: [["http://thesassway.com/intermediate",Sass.com]]
advanced_href: [["http://thesassway.com/advanced",Sass.com]]
wikipedia_href: [["https://en.wikipedia.org/wiki/Less_(stylesheet_language)",Less],["https://en.wikipedia.org/wiki/Sass_(stylesheet_language)",Sass]]
---

##First impression
My first impression of pre-compiled CSS, was "unecessary", but after trying SASS I have
changed opinion. It makes life way easier, for example to be able to nest tags in classes is very
useful and makes the code cleaner.

###Techniques

####Nesting
Sass allows you to nest tags and classes. Which is useful in cases when you for example, like to give p-tags
and h1-tags inside a specific layout you can nest them inside that tag instead of writing separate css rules for each nesting.

####Variables
Instead of using numbers you can assign values to variables and use in your code. It's a lot easier to remember
 $green-dark or $background-color instead of a hex-number. In this case $green-dark is asssigned the hex-value \#617643


