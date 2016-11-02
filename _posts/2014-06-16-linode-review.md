---
title: My experience transitioning from MediaTemple to Linode
date: 2014-06-16 00:00:00 Z
permalink: "/personal/mediatemple-to-linode-transition/"
categories:
- personal
tags:
- linode
- hosting
author: admin
layout: post
---

tldr; [Linode][1] offers great value and I highly reccomend them ! 

I have been a [Mediatemple][2] customer for the past 7 years - since 2007. I started with their Grid service and then migrated to a 1GB DV a few years ago. My migration to DV was prompted by constant decrease in performance that I was experience on their grid. Performance issues were solved after migrating and actually they have been very accommodating when I had to migrate. I think they actually helped me with the migration.

I don't host a lot of websites and the websites that I have are not hight profile - highly trafficked websites. So I always felt like paying ~$45/month for hosting is a bit too much. Their smallest DV plan is $50/month but I had a 20% discount so it ended up being $40/month + $5/month for an extra IP.

I don't think the Godaddy acquisition changed anything with their service but I really wanted to pay less for hosting so I started looking for other options.

It was a little bit daunting to migrate all my websites but I decided to make the switch to Linode. I settled on the <strong>2GB plan</strong> (2GB RAM, 2 CPU cores, 48 GB SSD storage) which is (at the time of the writing) $20/month.

In order to get something from MT you'd have to pay $50/month so that's a substantial saving.

### What I like so far

The <strong>migration was painless</strong>. Their documentation is great and easy to follow. Even if you don't have a lot of experience administrating a server you should be able to follow along and set up everything.

<strong>The Speed</strong>: I always had problems with slow [Time to First Byte][3]. This can be caused by different reasons but since migrating to Linode my TTFB has improved significantly. One service that you can use to test that is [webpagetest.org][4] .

<strong>Their support:</strong> is really great. Mediatemple is known to have great support but I haven't experienced anything less from Linode.

<strong>Price</strong>: I am sure you can get cheaper hosting but their offering is really good. They don't charge an arm and a leg for extras either.

The price comparison below is for (roughly) the same setup - 2GB of RAM

<table>
  <thead>
    <tr>
    	<th></th>
      	<th>Linode</th>
      	<th>MediaTemple (DV Developer)</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
    	<td>Monthly:</td>
      	<td>$20</td>
      	<td>$50</td>
    </tr>

    <tr>
    	<td>Snapshot backups:</td>
      	<td>$5/month</td>
      	<td>$20/month</td>
    </tr>

    <tr>
    	<td>Extra IP:</td>
      	<td>$1/month</td>
      	<td>$5/month</td>
    </tr>
  </tbody>
</table>

### What I dislike

They don't make it clear that the backups are an extra add-on. It comes bundled with your plan and you have to pay extra for it. The price is worth keeping it though ($5/month for the 2 GB plan)

Conclusion: You need to be familiar or have the willingness to become familiar with Linux and the command line in order to manage your server. The price is right and add-ons like extra ips or backups are inexpensive. The performance is great.  

Linode just introduced a [1GB plan for $10/month][5], a great deal.


Further reading:


* [linode documentation][6]
* [Set up your linode for maximum awesomeness][7]
* [Setting up an outgoing mail server][8]

[1]:https://www.linode.com/?r=72d496fd6f3f292b4ffb371d9ea0cc04fc93a103
[2]:http://mdtm.pl/1n6YCUC
[3]:http://en.wikipedia.org/wiki/Time_To_First_Byte
[4]:http://www.webpagetest.org
[5]:https://blog.linode.com/2014/06/16/11th-linode-birthday-10-linode-plan/
[6]:https://library.linode.com
[7]:http://feross.org/how-to-setup-your-linode/
[8]:http://georgebuckingham.com/blog/php-outgoing-mail-ubuntu