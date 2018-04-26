---
title: Recommendations on VoIP/video chat tools
keywords: secure communications, voice calls security, video calls security, VoIP
last_updated: April 26, 2018
tags: [secure_communications, articles, faq]
summary: "Client uses Skype, Google Hangouts, or other commercial services for sensitive voice/video chat."
sidebar: mydoc_sidebar
permalink: voip_video_chat_tools.html
folder: mydoc
---


# Recommendations on video chat tools
## Secure solutions for voice/video calls

### Problem

Skype is not a good solution for human right defenders at risk.

Depending on their threat model, we should also discourage at-risk users from using other commercial services like Google Hangouts.


* * *


### Solution

#### 1:1 video calls

For end-to-end encrypted 1:1 voice and video calls, we can recommend:

- **Wire** - an open source desktop and mobile app for end-to-end encrypted messaging (both 1:1 and group) and calls (only 1:1) that doesn't need a telephone number to sign up.
    - [Wire website](https://wire.com)

- **Signal** - an open source desktop and mobile app for end-to-end encrypted messaging (both 1:1 and group) and calls (only 1:1).
    - [Signal announcement of video calls feature](https://signal.org/blog/signal-video-calls/)



#### Multi-party video calls

Currently there is no solution for end-to-end encrypted group calls.

For a group call to be as secure as possible, TLS/HTTPS needs to be implemented.

We should also warn our clients that, since group video calls are not end-to-end encrypted, their security depends on the entity that is hosting the service, so we should recommend primarily services that are hosted by trusted partners, or self-hosted.

- **Jitsi Meet** is a video conference browser-based option. It was developed by the same team of Jitsi, the desktop voice and messaging client. The main difference is you don't need to install a client for your computer, since you will connect using your browser to a trusted partner Jitsi Meet server. You can try this solution simply by going to [the Jitsi Meet official website](https://meet.jit.si).

    Since this service is not end-to-end encrypted, we should recommend an instance of Jitsi Meet hosted by a trusted partner. For example:

    - [meet.mayfirst.org](https://meet.mayfirst.org)
    - [meet.equalit.ie](https://meet.equalit.ie/)

    If the client has tech capacities, they can also choose to self-host a Jitsi Meet instance. Instructions for installing Jitsi Meet in a server can be found [here](https://github.com/jitsi/jitsi-meet/blob/master/doc/quick-install.md).

- **Wire** - For video calls with fewer than 10 participants, we can recommend Wire. Group video calls on Wire *are not encrypted*, but the audio and video quality is pretty good and stable. Participants can connect through the mobile or desktop app.
    - [Wire website](https://wire.com)

- Other server-trusting proprietary solutions for multi-party calls include [appear.in](https://appear.in/), [talky.io](https://talky.io/), [GoToMeeting](https://www.gotomeeting.com), [Zoom](https://zoom.us/), and [Google Hangouts](https://hangouts.google.com).


#### Voice calls

If video is not strictly necessary, and bandwidth is low, it is worth proposing multi-party audio calls, for example with **Mumble**, an open source, low-latency, high quality voice chat software that can be self-hosted in the client's server.

- To use Mumble, the participants in the conversation need to install a client:
    - [Mumble for Windows, Mac, and Linux](https://wiki.mumble.info/wiki/Main_Page)
    - Plumble for Android: [Google Play](https://play.google.com/store/apps/details?id=com.morlunk.mumbleclient.free) - [F-Droid](https://f-droid.org/packages/com.morlunk.mumbleclient/)
    - [Mumblefy for iOS](https://itunes.apple.com/dk/app/mumblefy/id858752232?mt=8)

- Mumble servers managed by trusted parties:
    - kefir.red  (Mexico) - [Instructions in Spanish](https://wiki.kefir.red/Mumble)
    - mumble.contaminati.net (Italy)
    - fala.navemae.xyz (Brazil) - [Instructions in Portuguese](https://wiki.ativismo.org.br/index.php?title=Mumble)
    - mumble.riseup.net (USA)
    - mumble.codigosur.net (Costa Rica)
    - [talk.systemli.org](https://www.systemli.org/en/service/mumble.html) (Germany)

- [Instructions for installing Mumble in a server](https://wiki.mumble.info/wiki/Installing_Mumble)
- If the Mumble conversation needs to be password-protected, a private channel can be created. To create a private channel, right-click when you connect to Mumble and set the name and a password for the channel. When you leave the channel, the logs and conversation disappear.


* * *


### Comments

[Greenhost's](https://greenhost.nl/) [Eclips.is](https://eclips.is) platform has a
pre-configured setup to launch a Meet Jitsi instance on their cloud.

[rocket.chat](https://rocket.chat/) - an open source fully featured slack clone - has plugins for WebRTC videobridging and OTR-encrypted chat conversations. It can be self-hosted as a standalone, or within a sandstorm.io instance, and could be more useful for organizations looking to consolidate Slack-style communications with a voice option.
