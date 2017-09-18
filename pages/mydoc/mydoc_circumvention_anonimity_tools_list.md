---
title: Circumvention & Anonimity tools list
tags: [article, support]
keywords: assessment, censorship, circumvention
summary: Best and secure circumvention tools, Tor, VPN, Tails
sidebar: mydoc_sidebar
permalink: mydoc_circumvention_anonimity_tools_list.html
folder: mydoc
---

# Circumvention & Anonimity tools list
## Best and secure circumvention tools, Tor, VPN, Tails

### Problem

- The traffic can be monitored by the government on different points of the
  path. 
- The client is suffering from online censorship.


### Solution

We need to understand the exact needs of the client, even if they have already
mentioned a specific tool. 

There are different ways of circumventing Internet censorship, some of which
provide additional layers of security. The tool that is most appropriate for the
client depends on their threat model and their specific need.


#### Initial evaluation

We need to assess and understand the threats the client is facing, and evaluate
how we can respond. 


##### Questions for the client

- What is the client's primary need? Are they interested only in circumvention,
or are privacy and anonymity also important?
- What data is being censored that the client wants to view? What is the
censorship context of his/her country?
- What appropriate tools are available and work in their country?
- In certain repressive regimes, the usage of VPNs or other tools might be
illegal. If you are unsure, you can involve the policy team for guidance, and
consult with Helpline management.
- If the client is asking how to hide their identity:  - we need to know what
they want to hide: just IP location, internet navigation, or more?
- Why do they need to hide their identity?


#### Best Practices

These are best practices we should explain to the client:

At first, we need to advise the client to use **HTTPS** - the secure version of
the HTTP protocol used to access websites.

[This HTTPS Everywhere plug-in may be an easy install](https://www.eff.org/https-everywhere)

In addition to the obvious benefits of HTTPS, there is a chance that the
encrypted version of the site is not blocked. 

Check the mobile and laptop website versions are both blocked.  For example,
instead of visiting https://twitter.com, we could visit https://m.twitter.com,
the mobile version of the site. Censors that block websites or web pages usually
work from a blacklist of banned websites, so anything that is not on that
blacklist will get through.

#### Circumvention & anonymity
##### Warning for every Tor-based tool

Before starting to use Tor, the client should check that their connections are
really anonymised: https://check.torproject.org/

[More warnings](https://www.torproject.org/download/download.html.en#warning)

In a nutshell:

- Don't open documents downloaded through Tor while online. These documents can
contain Internet resources that will be downloaded outside of Tor by the
application that opens them
- Web browsing is much slower than through a normal browser or a VPN because
your traffic is encrypted and relayed through the Tor network, but it shouldn't
be crippling. If you find it's too slow, you can try to change the circuit in
Tor Browser with Ctrl+Shift+L (with Orbot you can switch to a new identity by
swiping from right to left or from left to right on the onion icon)  -
https://tor.stackexchange.com/questions/8673/tor-browser-bundle-tbb-new-circuit-versus-new-identity
- Flash and many other features of websites won't work, for example you may not
be able to watch videos - this is a drawback, but enabling these features may
compromise your anonymity. Some websites, including Youtube, support HTML5
players when Flash is not supported by the browser and sometimes you can watch
the video by switching to the HTML5 version - https://www.youtube.com/html5
- You shouldn't log into accounts that can identify you through Tor, and you
should switch off geolocation if you're using a device that supports it
- Don't disactivate plugins and don't install other plugins in Tor Browser or
in Orfox/Orweb - use the default settings

- [Tor FAQ](https://www.torproject.org/docs/faq.html.en) - In particular: - [Why
is Tor so slow?](https://www.torproject.org/docs/faq.html.en#WhySlow)
- [How can I tell that Tor is working, and that my connections are really
anonymized?](https://www.torproject.org/docs/faq.html.en#IsItWorking)
- [Does Tor remove personal information from the data my application sends?](https://www.torproject.org/docs/faq.html.en#NoDataScrubbing)
- [Why can't I view videos on some Flash-based sites?](https://www.torproject.org/docs/faq.html.en#TBBFlash)

- [Understanding and Using Tor - An Introduction for the Lay(wo)man](https://trac.torproject.org/projects/tor/wiki/doc/)

* * *

**This is a list of some circumvention tools listed from a higher risk threat model to lower:**

#### Tails

**Tails** is a live operating system that you can boot on almost any computer
from a DVD, USB stick, or SD card.

It aims at preserving your privacy and anonymity, and helps you to:

- Use the Internet anonymously
- Circumvent censorship
- Leave no trace on the computer you are using unless you ask explicitly
- Use state-of-the-art cryptographic tools to encrypt your files, emails and
instant messaging

1. [Website](https://tails.boum.org/)
2. [Interactive Guide](https://tails.boum.org/install/index.en.html)

##### Warnings

-  If you use Tails, all traffic is routed through Tor and default applications
have been enhanced to protect your anonymity
- [Warnings for Tails](https://tails.boum.org/doc/about/warning/index.en.html)


#### Whonix

**Whonix** is a complete operating system designed to be used in a virtual
machine.

Designed for advanced security and privacy, Whonix mitigates the threat of
common attack vectors while maintaining usability. Its fail-safe, automatic,
and desktop-wide use of the Tor network allows for censorship circumvention and
anonymity. A heavily reconfigured Debian base is run inside multiple virtual 
machines, providing a substantial layer of protection from malware and IP 
address leaks. Commonly used applications are pre-installed and safely
pre-configured for immediate use.  

- [Website](https://www.whonix.org/)

##### Warnings

- If you use Tails or Whonix, all traffic is routed through Tor and default 
applications have been enhanced to protect your anonymity. 
    - [Warnings for Whonix](https://www.whonix.org/wiki/Warning)


#### Tor Browser

**Tor Browser** is software that protects you by bouncing your communications
around a distributed network of relays run by volunteers all around the world.
In certain locations, where connections are slow, it might be difficult to
establish the circuit through the Tor network.

1. The Tor Browser lets you use Tor on Windows, Mac OS X, or Linux without
needing to install any additional software. It can run off of a USB flash drive
2. [Official website](https://www.torproject.org)
3. Security in a Box has an updated guide on Tor Browser:
    - [Windows](https://securityinabox.org/en/guide/torbrowser/windows/)
    - [Linux](https://securityinabox.org/en/guide/torbrowser/linux/)
    - [Mac](https://securityinabox.org/en/guide/torbrowser/mac/)

##### Warnings

Please keep in mind that if you're using Tor Browser, only your activity within
the Tor Browser is encrypted and anonymised - any other internet traffic is not.
Other applications, like Skype or the regular browsers, will not be routed
through the Tor network, even if the Tor Browser is running.

#### Orbot

**Orbot** is an anonymity tool for mobile devices.

Available only for Android.

- [Website](https://guardianproject.info/apps/orbot/)
- Security in a box [guide on Orbot](https://securityinabox.org/en/guide/orbot/android/) 

##### Warnings

- If you use Orbot, by default only applications aware of Orbot such as Orfox
will be anonymised.
- You can also run Orbot in "VPN Mode" which will route all phone traffic 
through Tor. Be aware that there is a lot of identifying information that
applications (and your phone) transmit, so this is not a sufficient way to 
achieve anonymity on the phone. To enable the "VPN Mode", open the side panel
and click on the button next to "Apps VPN Mode".

*If needed we can mention that you can also torify your connections for some
selected apps that are not anonymised by default [Settings --> Select Apps in
v.15.2], but this requires root privileges on your device, so it's more
difficult and shouldn't be recommended to non experts.*


#### Onion Browser

**Onion Browser** is a free web browser for iPhone and iPad that encrypts and
tunnels web traffic through the Tor network, with extra features to help you
browse the internet privately.

Available only for iOS.

- Websites:
[1](https://blog.torproject.org/blog/tor-heart-onion-browser-and-more-ios-tor) -
[2](https://itunes.apple.com/us/app/onion-browser-secure-anonymous-web-with-tor/id519296448?mt=8)

##### Warnings: 

- Only connections through the Onion Browser are anonymised. Other applications
will not be routed through the Tor network, even if the Onion Browser is
running.
- Multimedia often bypass Tor and compromise your privacy; video files and
video streams are blocked by default and are not supported by Onion Browser.
- Use of Onion Browser is at your own risk; remember that sensitive
data does not always belong on a mobile device.

#### Orfox

A browser for Android that can be used to browse the Internet anonymously
together with Orbot (see above).

- [Website](https://guardianproject.info/apps/orfox/)

Orfox is built from the same source code as Tor Browser (which is built upon
Firefox), but with a few minor modifications to the privacy enhancing features
to make them compatible with Firefox for Android and the Android operating
system.

##### Warnings

- Use of Orfox is at your own risk; remember that sensitive data does not always
belong on a mobile device. See warnings for Orbot above.

### Circumvention

#### uProxy

**uProxy** is a browser extension that lets friends route their connection to
their Internet through each other’s computers. It can help people with
restricted or insecure access to the Internet get to the content they care
about safely.

- Websites: [1](https://jigsaw.google.com/projects/#uproxy) - [2](https://www.uproxy.org/)

#### FreeBrowser

**FreeBrowser** FreeBrowser is a free Android app that provides access to an
uncensored internet. Currently targeting Chinese users.

- [Website](https://freebrowser.org/en/)

#### Freenet

Freenet is a peer-to-peer platform for censorship-resistant communication and
publishing. Browse websites, post on forums, and publish files within Freenet
with strong privacy protections.

- [Website](https://freenetproject.org/)

#### VPN Providers

A **VPN** encrypts and sends all Internet data between your computer and another
computer. A VPN protects your traffic from being intercepted locally, but your
VPN provider can keep logs of your traffic (websites you access, and when you
access them). These logs could trace back to you, and if your adversary is
powerful enough, they could pressure VPN providers to disclose this information.

It is very important to trust the VPN provider you use. Some options are listed
below: 

#### Bitmask

**Bitmask** is A VPN client that uses Riseup and Calyx VPN servers. Depending on
their technical capacities, users could install this option on their own
server.

- Available only for Android and Linux users. Windows and Mac versions are
expected to be released soon.
- **Article #192** is dedicated to this tool and contains guides.
- [Website](https://www.bitmask.net)

##### Warnings

- [Limitations of Bitmask](https://leap.se/en/limitations)
- [Some security issues when using a VPN](https://riseup.net/en/vpn/security-issues)


#### Autistici VPN

This VPN service is recommended for high-risk activists but one needs to request
an account.

It is based on OpenVPN and can be used on Linux, Windows, Mac, Android and iOS.

- [This is the official website](https://vpn.autistici.org/)
- [Guide and resources](https://vpn.autistici.org/help/index-en.html)

*Note that Autistici's VPN is connected to the email account: if a mailbox is
never accessed for 6 months, it will be deactivated. The email account can be
then re-activated, but the user needs to contact Autistici's helpdesk to do so.
If the client is not interested in using Autistici's mail service, they should
rather use Bitmask.*

##### Warnings

- [Limitations to using Autistici's VPN](https://vpn.autistici.org/help/index-en.html#limitations-ai-vpn)


#### Riseup VPN Red

Besides its VPN based on Bitmask (VPN Black), Riseup offers also an
OpenVPN-based VPN service (VPN Red) recommended for high-risk activists.
To use Riseup VPN Red, one needs to [request an account on Riseup](https://account.riseup.net/user/new).

Riseup's VPN Red is based on OpenVPN and can be used on Linux, Windows, Mac,
Android and iOS.

- [Website](https://riseup.net/en/vpn/vpn-red)
- [Limitations of Riseup's VPN](https://riseup.net/en/vpn#limitations-to-using-the-riseup-vpn)
- [Some security issues when using a VPN](https://riseup.net/en/vpn/security-issues)

*This VPN is a bit more complicated to configure than Autistici's, but if the
client already has an account with Riseup, it will be probably faster to use
this.*

#### Mullvad

**Mullvad** is a VPN which incorporates some obfuscation tech.

- [Website](https://www.mullvad.net/)


### Circumvention Tools Based on Encrypted Proxies

These are proxy tools that utilize encryption. Although the connection is
encrypted, it might be traced back to you: these tools do not
provide anonymity. They are, however, more secure than a plain web-based proxy.
Examples of these tools include Lantern and Psiphon.

#### Psiphon

**Psiphon** is an award-winning circumvention system that uses a combination of
secure communication and obfuscation technologies.

1. Compatible with Android 2.2 and up.
2. Works on Windows XP, Windows Vista, Windows 7, and Windows 8 (desktop).
3. [Website](http://www.psiphon3.com)
4. [User guide](http://www.psiphon3.net/en/user-guide.html)

#### Lantern

**Lantern** is an Internet proxy tool. Its goal is providing access to the open
internet. Lantern is unique because it uses peer connections as a source of
internet connectivity when servers are unavailable.

1. Available for Mac, Windows, and Linux (desktop).
2. [Website](https://getlantern.org/)

### Web-based Proxies

This is a good way of circumventing censorship. Basically you route your HTTP
requests through a different computer (the proxy). The user must be careful,
since there are malicious proxy servers, capable of rerouting and modifying
users' requests for malicious purposes. 

Never use or trust a proxy server no one has ever heard of. And even if you
receive the proxy from a trusted partner, play it safe and do not pass on any
private information that isn't encrypted. 

- [A guide to use a web-based proxy](http://proxy.org/)


### Comments

- [Helpful article suggestion](https://ssd.eff.org/en/module/how-circumvent-online-censorship)

- Security in a box: [Remain anonymous and bypass censorship on the Internet](https://securityinabox.org/en/guide/anonymity-and-circumvention/)

- [Helpful comparison website for VPN](https://thatoneprivacysite.net/vpn-comparison-chart/)
