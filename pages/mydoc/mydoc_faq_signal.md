---
title: Signal FAQ for Organizations Using Signal 
tags: [faq, support, call-security, instant-messaging-security]
keywords: secure chat, secure voice, voice, call, secure call, text, texting, signal, Signal, text apps, apps for texting, encrypted text, encrypt text, android, ios, encrypted messages, encrypt messages
summary: This FAQ is to assist an organization interested in utilizing Signal, the secure text messaging app for Android and iOS, for their confidential text messages.
sidebar: mydoc_sidebar
permalink: mydoc_faq_signal.html
folder: mydoc
---


|Last Updated:|
|-------------|
| April 2016 |

   * [What is Signal?](#whatIs)
   * [Why should I trust it?](#trust)
   * [Where do I get it?](#where)
   * [How do I use it?](#how)
   * [Are all text messages encrypted?](#allMsg)
   * [Are all phone calls encrypted?](#allCalls)
   * [Is group messaging encrypted?](#groupMsg)
   * [Are group calls possible?](#groupCalls)
   * [Is it possible to accidentally send an unencrypted message?](#accidentMsg)
   * [Is it possible to accidentally make an unencrypted call?](#accidentCall)
   * [How do I know my call is secure?](#accidentCall)
   * [How do I know if my message was received?](#msgReceived)
   * [Does Signal use data/wifi for calls and messages?](#data)
   * [Can I send an insecure message if I have to?](#noSignal)
   * [Can I send messages to people who don’t have Signal?](#noSignal)
   * [Can I use my laptop/desktop to continue my conversations with Signal?](#signalDesktop)
   * [Are there cool things besides security features?](#coolFeatures)
   * [My question isn’t here](#question)


<a name="whatIs"></a>What is Signal?
-------------------------------------
Signal is an encrypted texting and voice chat app for iPhone and Android devices by the free and open source software team, [Open Whisper Systems](https://whispersystems.org/). The app allows you to message individuals or groups, make calls over the internet, and send pictures, videos or audio. 

You may be familiar with TextSecure and Redphone, which were secure texting and voice communications apps for Android. Signal replaces these apps and combines their functionality!
 

<a name="trust"></a>Why should I trust it?
------------------------------------------
Signal is open-source (their code is on [GitHub](https://github.com/whispersystems) for all to see), peer reviewed, and endorsed by security giants like Bruce Schneier and privacy advocates like Edward Snowden.

It is simple to install, simple to use, and provides end-to-end encryption.

 
<a name="where"></a>Where do I get it?
--------------------------------------
Download Signal from the Google Play Store or Apple App Store just as you would any other app. Please note, Signal is only available for Android and iOS.


<a name="how"></a>How do I use it?
----------------------------------
The EFF has some great resources for people using the app for the first time. The Helpline will also be available for questions and support as needed.

The guides lead you through installation, show you how to make an encrypted phone call, then how to use messaging. You will find it is very similar to other texting apps you’ve used! 

Android:
https://ssd.eff.org/en/module/how-use-signal-android

iOS:
https://ssd.eff.org/en/module/how-use-signal-ios 


<a name="allMsg"></a>Are all messages encrypted?
------------------------------------------------
All messages to other Signal users [are encrypted](http://support.whispersystems.org/hc/en-us/articles/213096658-How-do-I-know-my-message-is-private-) unless you manually change to an insecure message. Messages to non-Signal users are not encrypted, and you will be notified when you attempt to send a message to a non-Signal user. 


<a name="allCalls"></a>Are phone calls encrypted?
-------------------------------------------------
Voice chat is always encrypted. This feature can only be used with another person who has Signal installed. Note that your call quality is dependent on your internet connection, so it is recommended to make calls within wifi zones. 


<a name="groupMsg"></a>Is group messaging encrypted?
----------------------------------------------------
Yes, as long as [everyone in the group uses Signal](http://support.whispersystems.org/hc/en-us/articles/213707958-How-do-I-start-a-group-chat-When-is-it-a-Group-MMS-When-is-it-a-Group-over-data-).

If someone in your group does not have Signal, you will receive a pop-up warning that your added recipient does not have the app, and your message will be sent as an unencrypted MMS.


<a name="groupCalls"></a>Are group calls possible?
--------------------------------------------------
No, you are unable to add multiple parties to a Signal voice chat. There is currently not a solution for multi-party end-to-end encrypted voice or video communications. If the material is not sensitive, consider using Hangouts, Jitsi Meet, or a normal phone call depending on the level of sensitivity.


<a name="accidentMsg"></a>Is it possible to accidentally send an unencrypted message?
------------------------------------------------------------------
Not really. Secure messaging is the default. To [create an unencrypted message](http://support.whispersystems.org/hc/en-us/articles/212535548-How-do-I-send-an-insecure-SMS-), you must manually long-press the blue “Send message” arrow button until it changes from blue to gray, and the padlock unlocks.

However, **you must turn encryption back on after turning it off**, unless you close the conversation in which you turned it off. 

In group chat, it is a little easier to accidentally send a message unencrypted because if a member of the group does not have Signal, the message will not be encrypted. However, you 
will be notified when you’ve added a member who does not have the app.   


<a name="accidentCall"></a>Is it possible to accidentally make an unencrypted call? Or How do I know my call is secure?
--------------------------------------------------------
Calls are automatically encrypted, and you are able to double check the safety of this encryption using the generated words at the bottom of your call screen.

The two, highly different, words at the bottom of your call screen will be shown on both your phone and the receiver’s phone. They allow you to see if your call has been intercepted. If the call is compromised, you and your receiver will see different sets of words. 

In practice, this looks something like the following:

* Alice calls Bob. Alice notices the words *Aardvark Combatant* at the bottom of her call screen. She says to Bob, “The first word is *Aardvark*.” Bob replies, “The second word is *Combatant*” at which point Alice and Bob know their call is secure because they both see the same words. 

* If, on the other hand, Alice said “The first word is *Aardvark*.” and Bob replies “I don’t see *Aardvark* at all, my words are *Tissue Rainbow*.” Alice and Bob know their call is not secure, and they should hang up. 


<a name="msgReceived"></a>How do I know if my message was received?
------------------------------------------------------------------
[On Android](http://support.whispersystems.org/hc/en-us/articles/212535538-How-do-I-know-if-a-message-has-been-delivered-), the checkmarks at the bottom of each message indicate if your message was sent (one checkmark) and received (two checkmarks). 

Note that two checkmarks does not indicate if your recipient read your message, only that their device received it.

[For iOS](http://support.whispersystems.org/hc/en-us/articles/212535538-How-do-I-know-if-a-message-has-been-delivered-) users, the message will read “delivered” at the bottom. Once again, this does not indicate if the recipient has read the message, only that your recipient’s device has received it.


<a name="data"></a>Does Signal use data/wifi for calls and messaging?
---------------------------------------------------------------------
Yes, Signal makes calls and delivers messages over the internet. This means that Signal doesn’t cost any money (unlike SMS), allowing international communications for our global organization, if you have a data plan or wifi.

Please note call quality is very much affected by your internet connection in Signal; if you are having trouble connecting, consider moving to a wifi zone.

Also consider data cost when connecting with Signal. International travellers should be aware that using Signal may incur data charges when outside of their usual network.

Open Whisper Systems provide the following reference for data use:  "Voice calls use about 8 kilobits per second. So for 15 minutes expect 900KB (kilobyte). This brings your 30, 45, and 1 hour conversations to 1.8MB, 2.7MB, and 3.6MB, respectively."


<a name="noSignal"></a>Can I send an insecure message if I have to? Or can I send messages to people who don’t have Signal?
-------------------------------------------------------------------
iOS: 
Signal will only allow you to send texts to other people who have Signal. iOS users can use the default texting app Messages to send insecure messages or SMS to users who don’t have Signal.

Android:
Yes, but before you do, consider encouraging the receiver’s use of Signal as well - every new user means security becomes habit and the practice becomes normalized.

If you write a message to someone without Signal, you will be notified that your message is insecure, but you will not be prevented from sending a message.

[To send an insecure message](http://support.whispersystems.org/hc/en-us/articles/212535548-How-do-I-send-an-insecure-SMS-), long-press the blue arrow button, and select the gray arrow, reading “insecure”. 


<a name="signalDesktop"></a>Can I use my laptop/desktop to continue a conversation with Signal?
--------------------------------------------------------------------
[The beta](https://whispersystems.org/blog/signal-desktop/) for this feature opened Dec. 2, so go ahead and sign up if you feel adventurous! Otherwise, stay tuned for updates from the Tech Team about when it will be ready for primetime.


<a name="coolFeatures"></a>Are there any cool things besides security features?
-------------------------------------------------------------------
Yes! Signal has emojis, allows you to send videos and pictures, change the theme to black with white letters (if you have an amoled screen, it saves on battery!), and allows you to change the color of your contacts’ messages.

If you are looking for something, and Signal is not meeting your needs, please let the Helpline know.


<a name="question"></a>My question isn’t here.
---------------------------------------
Try Signal’s fabulous [FAQ](http://support.whispersystems.org/hc/en-us).


