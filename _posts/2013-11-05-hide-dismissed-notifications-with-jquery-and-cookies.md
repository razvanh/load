---
title: Hide dismissed notifications with jQuery and cookies
author: admin
layout: post
permalink: /javascript/hide-dismissed-notifications-with-jquery-and-cookies/
categories:
  - javascript
tags:
  - "dismiss alert"
  - "hide dismiss alert"
---
It&#8217;s quite easy to write a jQuery or plain JS script that dismisses an alert message but sometimes you want a little bit more. Usually that is to keep that notification hidden when you refresh the page. that can be done using various approaches and one of them is to use cookies. It&#8217;s as simple as setting/updating a cookie that contains a string with the ids of the notification containers that were dismissed.

Here&#8217;s an example of the html and JS.

<script src="https://gist.github.com/razvanh/7322236.js"></script>

<script src="https://gist.github.com/razvanh/7322262.js"></script>

This uses jQuery but can be easily rewritten to have no dependencies.  
If you have a better way of doing this, or any comments, please let me know!

A <a href="http://codepen.io/razvan/pen/oqiAt" title="Notification dismissal " target="_blank">demo</a> can be seen on CodePen.

## Get better with Javascript and JQuery:

Here are some books that will help you get better at Javascript and Jquery

* [JavaScript and JQuery: Interactive Front-End Web Development](http://www.amazon.com/dp/1118531647/?tag=greatdesignbo-20) 
* [JavaScript Patterns](http://www.amazon.com/dp/0596806752/?tag=greatdesignbo-20)



