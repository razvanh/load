---
title: Installing Let's Encrypt certificates on a Linode running Ubuntu 14.04 LTS
  and Apache
date: 2016-03-23 00:00:00 Z
permalink: "/linux/letsencrypt-linode-ubuntu/"
categories:
- linux
tags:
- ubuntu
- ssl certificates
- letsencrypt
- linode
author: admin
layout: post
---

I have a few domains hosted on my linode VM and I've been meaning to install ssl certificates for them. I had two options:

* Install a multi domain certificate for all of them
* Take advantage of the Apache SNI and install individual certs even if all domains share the same ip

I opted for the second variant and decided to use [Let's Encrypt](https://letsencrypt.org). The simplicity of the process really blew me away. It's almost magical. Here are the steps I followed:

1.Install git on your server (if it's not already installed)

```bash
$ sudo apt-get install git 
```
2.Install the Let’s Encrypt client. We will clone the Let’s Encrypt repository under /opt, which is a standard directory for placing third-party software on Unix systems

``` bash
$ sudo git clone https://github.com/letsencrypt/letsencrypt /opt/letsencrypt 
```
3.Set up the certificate. If you have multiple domains, repeat this step for each domain.

``` bash
$ cd /opt/letsencrypt
$ ./letsencrypt-auto --apache -d yourdomainname.com -d www.yourdomainname.com
```
4.Let's Encrypt certificates are valid for 90 days. If you don't feel like manually renewing each 90 days you can automate the renewal process using a crontab job:

Edit crontab:

``` bash
$ sudo crontab -e
```
Add the new job:

```
30 2 * * 1 /opt/letsencrypt/letsencrypt-auto renew >> /var/log/le-renew.log
```

5.Since the letsencrypt client is still in beta you should probably update it regularely:

``` bash
$ cd /opt/letsencrypt && sudo git pull
```