---
layout: post
title: "Manual install of a nextcloud app"
date: "2021-02-07 03:36:22 -0500"
description: When native install is giving the piss... # Add post description (optional)
img:  nextcloud.png # Add image post (optional)
tags: [nextcloud, apps, handrolled,] # add tag
---

# Recently when updating nextcloud version's I noticed some apps weren't making it through to the other side. #

In particular the nextcloud social app was missing after an update. When I tried to reinstall it from my clouds appstore it was giving me a failed to extract error.

 So this is more of a workaround that I've been using in the meantime to manually install and activate it.

## The steps ##

 You will need ssh access to your cloud server and root.

 {% highlight console %}
 user@cloud:$ sudo su
 root@cloud:# cd /var/www/nextcloud/apps
 # wget https://github.com/nextcloud/social/releases/download/v0.4.2/social-0.4.2.tar.gz
 # tar -zxvf social-0.4.2.tar.gz
 # rm social-0.4.2.tar.gz
 # chown -R www-data:www-data social
 # cd ..
 # sudo -u www-data php occ app:enable social
 {% endhighlight %}

 * Just to clarify `sudo su` to become root.
 * Then change to your nextcloud installations apps directory.
 * You can use wget to download the apps tar.gz release file from github.
 * extract the file with `tar -zxvf`
 * remove the compressed file
 * set proper permissions with `chown`
 * use occ to enable app.
