---
title: Stop youtube videos when dismissing the bootstrap modal
author: admin
layout: post
permalink: /personal/stop-youtube-videos-when-dismissing-the-bootstrap-modal/
categories:
  - javascript
  - Personal
  - Web design
tags:
  - bootstrap
  - jquery
  - modal
  - youtube
---
I was working on a project that uses bootstrap as a foundation and some youtube videos are played using a modal window. The problem we encountered is that the videos kept playing in the background even after the modal was dismissed. Here is a simple solution to this problem, using jQuery &#8211; clear the &#8220;src&#8221; of the iframe and add it again so you can see the video again if you want to.

<script src="https://gist.github.com/razvanh/5767054.js"></script>

## Get some Javascript and Jquery help

Here are some books that will help you get better at Javascript and Jquery

* [JavaScript and JQuery: Interactive Front-End Web Development](http://www.amazon.com/dp/1118531647/?tag=greatdesignbo-20) 
* [JavaScript Patterns](http://www.amazon.com/dp/0596806752/?tag=greatdesignbo-20)


