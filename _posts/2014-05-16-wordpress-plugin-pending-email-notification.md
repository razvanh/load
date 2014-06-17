---
title: Simple wordpress plugin for email notifications of pending submissions
author: admin
layout: post
permalink: /wordpress/email-notification-pending-submission-plugin/
categories:
  - wordpress
tags:
  - wordpress email notification pending submission
  - wordpress plugin
---
![email notification for pending wordpress submissions](/images/psm.jpg)

I am working on implementing of Wordpress for an online publication that has a large editorial staff. There are a few admins and a lot of contributors that can submit articles. 

When a contributor submits an article, it goes to a submission queue that has to be reviewed by an admin. 

The problem is that there is no email notification when this happens. The admin gets an email when a new comment is awaiting moderation but there is no email for pending article submissions. I think this is an important oversight - more robust email notifications should be part of core wordpress.

I built a very simple plugin that will send out an email when a new article is submitted for review. The contributor will also receive an email when/if his article is published. I also added a settings page in the admin where you can set the email(s) to be notified.

Download it on [github][1] or feel free to create a pull request if you feel like improving it :)

[Wordpress.org plugin page][2]

 [1]: https://github.com/razvanh/simple-wp-notify-pending
 [2]: http://wordpress.org/plugins/pending-submission-notifications/