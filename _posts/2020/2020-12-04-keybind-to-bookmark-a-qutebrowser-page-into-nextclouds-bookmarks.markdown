---
layout: "post"
title: "Keybind to Bookmark a qutebrowser page into nextclouds bookmarks"
date: "2020-12-04 06:14"
---

Gmornin
just posting a simple binding I was trying to figure out to get qute browser to auto load my nextcloud instances bookmark capture utility.
so with this keybind you will be able to send the page you are on to your nextcloud instance to be saved as a bookmark.

``` :bind <key> open javascript:(function()%7Bvar%20a=window,b=document,c=encodeURIComponent,e=c(document.title),d=a.open('https://YOURNEXTCLOUDURL.com/apps/bookmarks/bookmarklet?url='+c(b.location)+'&title='+e,'bkmk_popup','left='+((a.screenX%7C%7Ca.screenLeft)+10)+',top='+((a.screenY%7C%7Ca.screenTop)+10)+',height=500px,width=550px,resizable=1,alwaysRaised=1');a.setTimeout(function()%7Bd.focus()%7D,300);%7D)(); ```

Be sure to edit `<key>` to the key you wish to bind.
as well as `YOURNEXTCLOUDURL.com` to point to your actual nextcloud instance.
