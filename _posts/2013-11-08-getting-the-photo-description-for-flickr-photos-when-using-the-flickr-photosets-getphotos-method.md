---
title: Getting the photo description for Flickr photos when using the flickr.photosets.getPhotos
  method
date: 2013-11-08 00:00:00 Z
permalink: "/php/getting-the-photo-description-for-flickr-photos-when-using-the-flickr-photosets-getphotos-method/"
categories:
- php
tags:
- flickr
- flickr.photosets.getPhotos
author: admin
layout: post
---

While their documentation does&#8217;t mention anything about this, it is possible to retrieve photo descriptions when using **flickr.photosets.getPhotos**.  
All you need to do is add &#8220;description&#8221; as an extra parameter. You can test it [here][1]. Below is the php code.

<script src="https://gist.github.com/razvanh/7373142.js"></script>

 [1]: http://www.flickr.com/services/api/explore/flickr.photosets.getPhotos