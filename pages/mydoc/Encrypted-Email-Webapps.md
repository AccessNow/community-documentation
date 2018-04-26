---
title: Recommendations on encrypted email web apps
keywords: secure communications, email, email security, protonmail, tutanota, hushmail
last_updated: April 26, 2018
tags: [secure_communications, articles]
summary: "A client is asking for a review of a specific secure web application for encrypted email, e.g. Tutanota, Protonmail, Hushmail."
sidebar: mydoc_sidebar
permalink: encrypted_email_webapps.html
folder: mydoc
---


# Recommendations on encrypted email web apps
## General advice on web applications for encrypted email - Tutanota, Protonmail, Hushmail

### Problem

A client is contacting us asking for a review or recommendations about a specific web service providing a web app for encrypted email.

We need to provide general advice and warn the client about possible vulnerabilities in the application.


* * *


### Solution

1. The first thing we need to do is assess the needs and the situation of the client: if the client or the people they need to exchange encrypted messages with are operating in a high-risk context, we should recommend them other options for encrypting their emails, as described in article # : [Secure Email Recommendations](Secure_Email_Recommendations.md).

    If the client and their contacts are not operating in a high-risk context, we can consider a web app for encrypting email a reasonable tool for protecting their privacy.

2. Gather information about the application, check its website, look at online reviews, audits, etc. It's also a good idea to check specialized mailing lists, for example: the [Modern Crypto mailing list](http://moderncrypto.org/mail-archive/messaging/). 

3. Analyze the application taking into consideration the following points:

    - Is the application mature? New applications/software are rarely good in regards to security. Before a piece of software can be deemed secure it needs to pass the test of time. Note that security applications and protocols have usually been around for a long time.
    - Is the application based on open software? Tutanota and Protonmail have free and open source mail clients, however their server software is not open source. Hushmail is proprietary software both on the client and the server side. We should recommend clients use free and open source software whenever possible if appropriate.
    - Web applications for secure email require the user to blindly trust the server that is providing them with secure code. An adversary might have the capacity to alter the code being served. Does the service have any mitigation in place?
    - Does the service provide a way to verify contacts' keys, or does it do automatic key discovery?
    - Are the users' private keys stored in the server? And if so, does the service have a way of protecting them so that they can only be accessed by the user?
    - Be wary of commercial audits, they are often very limited. If the audit is available, take a look, analyze it.
    - Look at the quality of key documents, such as the application's
    threat model.

4. Share your analysis and thoughts with the Helpline before replying to the client. Follow the approval process as established.


* * *


### Comments

1. 95% of all vulnerabilities in security applications are in
    their implementation, not in the crypto algorithms, etc. This is
    why the fourth dimension (time) is so important for security tools.
    There is almost no such thing as a new and secure security tool,
    because it takes some time of use, and testing, and research to
    identify the implementation flaws. We should always be extremely
    wary of advising anything but caution with regards to new
    applications.

2. Any commercial audits of commercial products should be looked into,
    because often these are very limited. For example often the vendor
    will make a statement/s about the product, and the auditing company
    is just verifying if those are true statements about the product or
    not. This is not very useful from a true confidence point of view
    with regards to the product. For example they will often say
    "Verify that product x has a key length of 2048 bits", the auditing
    company looks and verifies that indeed the product uses a keylength
    of 2048 bits, but makes no effort to test the implementation of key
    management within the application, etc.

3. Look at the quality of key documents, such as the application's
    threat model. It will tell you a lot about the depth of the team's
    security understanding and approach. If you can pick holes in the
    documentation then you will almost certainly be able to fly a
    Boeing 747 through the application.

So when a client comes to us and asks "Is new application x good?", we
should warn them that the application has not stood the test of time,
and therefore is almost certainly not secure. While the design and
crypto utilized may look secure, they need to understand that 95% of the
issues will not manifest in the design or crypto. Maturity is,
unfortunately, king when it comes to security tools. We also need to
keep this in mind with our own tools, such as IAS. This is also exactly
why innovation in security tools is so desperately needed, because what
we are innovating today, will perhaps become good security tools in 10
years time. On the flip side, if we are not innovating new tools today,
then we essentially know that we will not have any good and mature
security tools in 10 years!!

