---
title: How to circumvent the Great Firewall in China
keywords: anonymity, circumvention, VPN, Tor, China
last_updated: April 26, 2018
tags: [anonymity_circumvention, articles]
summary: "Client needs to overcome the Great Firewall in Mainland China."
sidebar: mydoc_sidebar
permalink: vpn_china.html
folder: mydoc
---


# How to circumvent the Great Firewall in China 
## VPN recommendations for Mainland China

### Problem

A client needs to circumvent the Great Firewall, either because they live, or are travelling to, Mainland China, but:

- VPN servers are frequently blocked in Mainland China.
- There is some evidence that the Great Firewall has the ability to selectively block VPN traffic.
- Some VPN providers do not respect users' privacy.
- Tor is blocked in Mainland China.

* * *


### Solution

#### VPNs

The solution we propose to the client will depend on what they need.

If the user is just interested in circumvention, they can use a VPN.

Sometimes some of these tools will work in some regions or circumstances and not
in others, and some of them may be blocked at the ISP level, so the best
strategy is to set up several VPNs before the client travels to China, so that
they have more than one option in case one doesn't work.

A good resource to identify available and functional VPN services in
China is [Great Fire](https://cc.greatfire.org/en).

From recent reports, we have seen that [AirVPN](https://airvpn.org/) works in
Beijing and [uProxy](https://www.uproxy.org/) works in Shanghai.

We can offer the client free accounts for AirVPN and uProxy.

#### Tor

In China Tor may be blocked, so it is important to add bridges, specifically
meek bridges, to the Tor setup. A howto for using meek bridges can be found
[here](https://trac.torproject.org/projects/tor/wiki/doc/meek).

The client should install Tor Browser before they travel, since the Tor project
page is blocked in China.

- Article on what to do when [Tor is blocked in a
  country](https://blog.torproject.org/blog/breaking-through-censorship-barriers-even-when-tor-blocked)
  - [FAQ on Tor bridges](https://bridges.torproject.org/)
  - [How to add bridges in the Tor Browser](https://www.torproject.org/docs/bridges#AddTorNotWorks)


* * *


### Comments

As of October 2017, AirVPN worked for phones in Beijing.  Several
circumvention tools (e.g. Lantern, ShadowSocks, ShadowSocks R, Psiphon, Tor) are
likely to be blocked in certain networks. vyprvpn (free version) and
AnchorFree (free version) worked in Beijing with a DSL broadband provided by
either China Telecom or a local provider, but not with video streaming, just for
emails and instant messaging.
