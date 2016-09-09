---
title: Two-Step Verification for Google Apps Organization FAQ 
tags: [faq, support, authentication]
keywords: 2fa faq, 2fa, two facotr, two step, 2 step, 2-step, Google, google, google apps, secure google, google account, verification, authentication
summary: This FAQ is to answer some common questions about two-step verification for organizations planning to implement it for their team's use of Google Apps.
sidebar: mydoc_sidebar
permalink: mydoc_faq_2fa_google_apps.html
folder: mydoc
---

|Last Updated:|
|-------------|
| April 2016 |


   * [What is it?](#whatIs)
   * [How is 2-Step different than Two-Factor Authentication (2FA)?](#diff2step2fa)
   * [Why do I want it?](#why)
   * [How do I start?](#how)
   * [Which authentication method should I choose?](#authenticationMethod)
   * [I already have 2-Step, but I did not use a One Time Password app for my authentication. How can I change the authentication method?](#changeAuthentication)
   * [How often will I have to use my second step for authentication?](#howOften)
   * [What happens if I lose the device with the One Time Password app or my security key?](#lost)
   * [What if I have no data or phone connectivity?](#travelling)
   * [What if I am travelling?](#travelling)
   * [What else does Google do with the phone number?](#whatElse)
   * [How do I remove trusted devices?](#removeTrust)
   * [Out of curiosity, what are the other options?](#options)
   * [What other accounts can I protect with 2-Step?](#protectAccounts)
   * [More Information](#moreInformation)


<a name="whatIs"></a>What is it? 
---------------------------------

Abbreviated as 2-Step, Two-Step Verification is a way to protect your account beyond a password. Two-Step Verification requires someone logging into an account to have two pieces of information that only the authentic user of an account is supposed to know. 

In Google’s case, an example would be a password and something else: a code generated with a One Time Password app, a text sent to the user’s phone, or a personal keyfob plugged in to your usb port. Only with both the password and the other factor can the user successfully log in.

Staff should be as secure as possible, so we will be choosing the One Time Password app (like Google Authenticator, FreeOTP, or OTP Authenticator) method of verification. This method also qualifies as Two-Factor Authentication, but “2-Step” will be used for the duration of the guide because it is the name used by Google.


<a name="diff2step2fa"></a>How is 2-Step different than Two-Factor Authentication (2FA)? 
--------------------------------------------------------------

2-Step is very similar to 2FA (Two-Factor Authentication), and often it is used as a straight synonym. However, 2FA is technically more involved. 

Like 2-Step, two pieces are necessary to log in to an account. A password still serves as the first piece; it’s something you know, information supposedly only known to the user. In 2-Step, the second piece is usually something you know also. In 2FA, the second piece is something you have (a physical item, like a phone or security key) or something you are (characteristics inherent to you, like a fingerprint or retina pattern).

Google’s SMS texts or voice message options are not things you have, but actually things you know, making them less secure and qualifying as only 2-Step processes. Luckily, the other options available, an OTP app or security key, do count as Two-Factor, and their greater level of security is why the team will be using One Time Password apps for verification.

This [handy flowchart](https://paul.reviews/the-difference-between-two-factor-and-two-step-authentication/) makes a quick visual of the difference.


<a name="why"></a>Why do I want it?
---------------------------------

A password can be compromised in myriad ways, and people often create rather poor passwords themselves. Without a secondary item needed for login, your personal email, documents, sheets, forms, shared projects, and any information you have in your Google account is more vulnerable. Your compromised account could then be used to compromise coworkers accounts or the broader community you work with.

Setting up 2-Step for your Google account helps avoid this single point of failure by providing a stronger line of defense for your account.


<a name="how"></a>How do I start?
----------------

   1. Visit the [2-Step Verification page](http://accounts.google.com/SmsAuthConfig). Be prepared to sign in.
   
   2. Click **Start setup** 

   3. Follow the instructions. During this process, you will be asked for your phone number to enable 2-Step. You may choose to remove the number later, after setup is complete.
   
   4. After receiving and verifying your account with the first code, you may choose to trust the computer you are using - assuming only you have access to it. This will prevent your having to [complete the 2-Step process every time](#howOften) you log in.
   
   5. Review your [settings](https://accounts.google.com/b/1/SmsAuthSettings#devices) and under “Verification Codes” choose a One Time Password app as the “Primary Way You Receive Codes”. Please read [Which Authentication method should I choose?](#authenticationMethod) for the rationale.  
 

<a name="authenticationMethod"></a>Which authentication method should I choose?
---------------------------------------------

Staff should use a **One Time Password app**, like [Google Authenticator](https://support.google.com/accounts/answer/1066447?hl=en), [FreeOTP](https://fedorahosted.org/freeotp/), or [OTP Authenticator](https://fossdroid.com/a/otp-authenticator.html). These are available on the Google Play Store, F-Droid, or Apple App Store for download and installation on a smartphone or tablet. 

Android:
* [Google Authenticator](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2)
* [FreeOTP](https://play.google.com/store/apps/details?id=org.fedorahosted.freeotp)
* [OTP Authenticator](https://play.google.com/store/apps/details?id=net.bierbaumer.otp_authenticator)

iPhone:
* [Google Authenticator](https://itunes.apple.com/us/app/google-authenticator/id388497605?mt=8)
* [FreeOTP](https://itunes.apple.com/us/app/freeotp-authenticator/id872559395?mt=8)

Please speak with the Helpline if you have concerns regarding this requirement.

**One Time Passwords (OTPs)** are one-time use codes generated by an app. Google offers [Google Authenticator](https://support.google.com/accounts/answer/1066447?hl=en) as one such option, but there are free-and-open-source (FOSS) options like [FreeOTP](https://fedorahosted.org/freeotp/) and [OTP Authenticator](https://fossdroid.com/a/otp-authenticator.html) as well. After generating the code in the app, simply type it in before the timer on the code runs out. Only the device with the authenticator app installed will be able to generate these codes, so as long as an attacker does not have your unlocked device at hand, you should be safe. This option does not require data or a phone connection.


<a name="changeAuthentication"></a>I already have 2-Step, but I did not use a One Time Password app for authentication. How can I change the authentication method?
---------------------------------------------------------------------------------------------------------------------------------

It’s easy to switch your verification choice. Go to your [2-Step Verification settings](https://accounts.google.com/b/1/SmsAuthSettings#devices) and register your One Time Password app as the new mode of authentication. 


<a name="howOften"></a>How often will I have to use my second step for authentication?
----------------------------------------------------------------

When you first try to sign in to your Google account on a new device you will be asked to complete the full two step process.

If the new device is a computer or phone that you own, and one that only you have access to, you may [choose “trust this computer”](https://support.google.com/accounts/answer/2544838?hl=en) to avoid the 2-Step process every time you sign in.

Without checking the “trust this computer” box, you will be asked for your second step every time you sign in to your account.


<a name="lost"></a>What happens if I lose the device with the One Time Password app or my security key?
------------------------------------------------------------------------------------

Use a [backup code](https://support.google.com/accounts/answer/1187538?hl=en) to sign in. These backup codes are provided on the Sign-in verification page when you enroll in 2-Step Verification. They act as backup one-time passwords for use in case you have lost the ability to use your OTP app. These codes should be written or printed and kept in a secure location.

Then, change your device or security key options in the [settings](http://accounts.google.com/SmsAuthConfig).


<a name="travelling"></a>What if I have no data or phone connectivity? Or what if I am travelling?
------------------------------------------------------------------------------------


One Time Password (OTP) apps, including Google Authenticator, do not require data or a phone connection to use, so just ensure you pack your device with the OTP app on it, even without a data plan. 

Before your trip, be sure to print [backup codes](https://support.google.com/accounts/answer/1187538?hl=en), generated in your settings page. Keep these with you just in case the device with the OTP app gets lost. These codes may only be used once, but you may print more whenever you need to.


<a name="whatElse"></a>What else does Google do with the phone number?
------------------------------------------------

[Nothing](https://support.google.com/a/answer/3563558). Your phone number will only be used to protect your account, and will never be sold, published, or called unsolicited. However, it will allow Google to associate your Google account with the phone that you use -- something Google has already done if you receive email on your phone.

<a name="removeTrust"></a>How do I remove trusted devices? 
---------------------------------

If you have a computer or phone registered as a trusted device that you would like removed, go to [My Account](https://myaccount.google.com/), Find “Sign-in & security” then choose Signing in to Google on the left. Find 2-Step Verification, and then click the “Registered Computers” tab. Choose “Require codes” for any device you would like removed from the trusted list.  


<a name="options"></a>Out of curiosity, what are the other options?
----------------------------------------------

| Note: |
|-------| 
| For the highest security, staff should use a [One Time Password application](#authenticationMethod) unless given personal instructions by the Helpline. |

A [security key](https://support.google.com/accounts/answer/6103523?hl=en) is a physical device you keep on your person. It’s a small plastic key-fob that you [purchase](http://www.amazon.com/s/?field-keywords=%22FIDO%20U2F%20Security%20Key%22) and insert into your computer’s usb port when logging in. It is very difficult to compromise your account with this option because the key will have to be physically taken to do so. A key does not require data or a phone connection to be used successfully, but you may not use it on a mobile device as a usb port is required. When being used for Google, this option only works in the Chrome web browser. A security key is something you have, and with your password, counts as the second step in a [Two-Factor Authentication](#diff2step2fa) process.

The **SMS text message** option sends a code to your phone to receive as a text. An advanced attacker may compromise this by intercepting the text and using the code before you receive it. In general, this is still a relatively safe option. Note you will need a data connection to receive the text. This counts as something you know, making your password and the text a [2-Step Verification](#diff2step2fa) process.

A **voice call** leaves a number code message on your phone’s voicemail system. If you do not have a PIN password set up to hear your voicemail, this option is very unsafe. Without a PIN, anyone can access your voicemail with minimal knowledge, requiring only your phone number and carrier to listen. This option will require a signal to receive the call, and is only as safe as your voicemail passcode. A message counts as something you know and, with the password, a [2-Step Verification](#diff2step2fa) process.


<a name="protectAccounts"></a>Great! My Google account is more secure. What else can I protect? 
-----------------------------------------------------------------

Many websites have a 2-Step Verification option. 
Find your favorites [here](https://twofactorauth.org/) or click the links for the following:
   * [Twitter](https://blog.twitter.com/2013/getting-started-with-login-verification)
   * [Facebook](https://www.facebook.com/notes/facebook-engineering/introducing-login-approvals/10150172618258920) 
   * [Amazon](https://www.amazon.com/gp/help/customer/display.html?nodeId=201962420)
   * [Dropbox](https://www.dropbox.com/en/help/363)


<a name="moreInformation"></a>Where can I find more information?
-----------------------------------

Google has a [how to and question list](https://support.google.com/accounts/topic/28786?hl=en&ref_topic=3382253) for 2-Step, and the [EFF’s guide](https://ssd.eff.org/en/module/how-enable-two-factor-authentication) is a great overview. 

