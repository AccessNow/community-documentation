---
title: Website down
keywords: website protection, infrastructure, intrastructure security
last_updated: April 26, 2018
tags: [infrastructure, articles]
summary: "A website is unreachable."
sidebar: mydoc_sidebar
permalink: website_down.html
folder: mydoc
---


# Website down
## How to track an issue when a website is down

### Problem

- Website is unreachable.


### Solution

- Check if the website is online from your end, as it could be censored
in the client country. You can use http://www.isup.me/
- Check the website of the host provider, as it could be the provider who is 
  facing some technical issues
- Check if there is any error message. It could be a software issue
- It could be a campaign against a type of websites that support the same cause.
  Check the availability of the other websites.
 
Some tests could be done to track the issue:
* ping the website and see if ping returns an IP or not
* nmap it, to find which ports are working
* Whois it, to identify the location of the admin, the host provider, etc.
* Reverse its IP to find out if the website is co-hosted
* if the site is co-hosted, find out if the other websites are down too or not

Based on the results of these tests, we can figure out if the connection
request is being turned down by the ISP, or censored by the authorities, or if
the website is down due to a DoS attack, etc.

### Comments

[Reference](https://github.com/OpenInternet/MyWebsiteIsDown/blob/dev/MyWebsiteIsDown.md)

