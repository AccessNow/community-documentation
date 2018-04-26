---
title: Website censorship in China
keywords: censorship, circumvention, VPN, Tor
last_updated: April 26, 2018
tags: [censorship, articles]
summary: "A website is censored in China by the Great Firewall."
sidebar: mydoc_sidebar
permalink: website_censored_china.html
folder: mydoc
---


# Website censorship in China
## Ways to make a website censored by the Great Firewall accessible in Mainland China

### Problem

A website is censored in Mainland China by the Great Firewall.

The website is only unreachable within Mainland China, and the issue is not related to technical problems with the management of the website.

The website is reachable from other areas and works correctly. Therefore we will need to examine the client's capacity and the existing solutions to make the website accessible to its Chinese users.

The solution we identify needs to be affordable for the organization and should not compromise the accessibility of the website for other user bases.


* * *


### Solution

The first step we need to make is confirming that the website is inaccessible in Mainland China. These tools can be used to check if a website is blocked in China:

- https://en.greatfire.org/analyzer
- https://www.greatfirewallofchina.org/

Depending on the client's financial and technical capacities, we can suggest one of the following solutions:

- [Greatfire](Greatfire.org) can make the website available via an Android application, which will be available all over the world. However, they are expensive: USD 5,000 - USD 10,000 for the creation of the app, and then a monthly fee of USD 3000 which would include all hosting charges with a minimum contract period of one year. If the client is interested in marketing and promoting the app in China, they can also work out a marketing plan based on the client’s budget.

- Domain Fronting: This is a solution that can help circumvent the censorship, but it requires technical capacity to set it up, as well as the cost of a CDN service. It also implies that a new URL for the censored website will have to be publicized to the Chinese readers.

    Domain fronting is implemented using a CDN as a proxy. This is because a CDN’s front end server, on receiving a request for a resource not already cached, forwards the request to the domain found in the Host header (the “origin server”). The client issues a request that appears to be destined for an unrelated front domain, which may be any of the CDN’s domains that resolve to an edge server; this fronted request is what the censor sees. The edge server decrypts the request, reads the Host header and forwards the request to the specified origin.
    
    - [A technical explanation](http://www.icir.org/vern/papers/meek-PETS-2015.pdf)
    - [How to use domain fronting for censorship circumvention](https://medium.com/@pmvk/domain-fronting-a-technique-used-to-circumvent-internet-censoring-10ef1bb3db84)
    - [Domain fronting explained](https://www.parckwart.de/computer_stuff/domain_fronting_explained)

- [China Cache](https://en.chinacache.com/): A client has been suggested to use China Cache to serve content inside China.

- Switching domain names and hosting: This is the least efficient solution. It consists in mirroring the website on other domain names and hosting providers and switching to a new one every time the current one is blocked by the GFW. This will be highly obvious and will not use any mean to conceal the website from the censors, so eventually the new URL might be censored too. It takes some work to set it up, can be frustrating for the site's audience, may reduce the audience's trust in the site, and is usually short-lived.


* * *


### Comments


For circumventing the Great Firewall on the client's side, please refer to article [#110: How to circumvent the Great Firewall in China](../Anonymity_Circumvention/VPN_China.md).


