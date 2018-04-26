---
title: Client Receives a Suspicious/Phishing Email
keywords: vulnerabilities, malware, phishing, email
last_updated: April 26, 2018
tags: [phishing_suspicious_email, articles, faq]
summary: "The client has received an email with or without an attachment from a known or unknown source."
sidebar: mydoc_sidebar
permalink: suspicious_phishing_email.html
folder: mydoc
---


# Client Receives a Suspicious/Phishing Email 
## Guide for phishing/suspicious email cases

### Problem

The email may contain malware or a link to a malicious site that tricks the
client into disclosing personal information. 

The longer a malevolent website stays online, the more victims it will create.
Reporting this website is one of the most important steps the Helpline can take.


* * *


### Solution

1. Protect the client, and respond to their concerns. 

    Be sure to clearly state the email *should not be opened, nor a linked site
visited*. Use your response to ask for the full headers of the email. 

    [This link](https://www.circl.lu/pub/tr-07/) may be used to assist the client in locating the full headers for many
email clients (including Gmail, Yahoo, Thunderbird, and Outlook).

    If you need the raw email message (including attachments), consider sending the
client [this link](https://www.circl.lu/pub/tr-34/) to help them.

    The template for this step may be found [here](../Templates/Phishing-First_Email.md)

    NOTE: If the client has already visited a site, or opened an attachment, we
should increase the urgency and impact of the case. 

2. Ask if the supposed sender is known to the client.

3. After receiving the headers and full email source from the client in Step 1, analyze the following:
    - Where is the email coming from? From what Country, ISP, IP address?
    - Is the IP address part of the Tor network? Check [this link](https://www.dan.me.uk/tornodes)
    - Are there any links in the email?
        - Where are those links pointing to?
        - If you believe it to be in good judgment, get the full content of the site using WGET and/or CURL. Be sure to conceal your identity using Tor. (On Linux, use the command `torify wget -qO- -U curl ifconfig.me` to check your IP.)
        - Where is the domain registered?
        - Is a file downloaded on the link?
        - Is the website asking for personal information?
    - Are there any attachments?
        - Be careful opening the attachments.
        - Use a virtual machine for the analysis.
        - Run them through an antivirus.
        - Open docs or PDFs on web services.

    - Use this [header analysis tool](https://toolbox.googleapps.com/apps/messageheader/)

    - If the suspicious email was identified as Gmail scam, Please follow [this link](https://support.google.com/mail/answer/1074268?hl=en)

4. Communicate to the client the conclusions of your investigation, and if
necessary, report the website.



**Take Down a Corrupted Domain**
When there is a phishing website, it is important to get the page off of the
internet to avoid having more victims. 

One way to do it is to follow the instructions offered by [Circl CERT team](www.circl.lu):

1. Paste the link in [this page](https://www.circl.lu/urlabuse/) to receive all the contact points from the whois entries.

2. Send to *all contacts* listed an email notifying them of the malicious
content found on one of their domains. An example of what this email could look like may be found in [Template #209 - Phishing Link](../Templates/Phishing_Link.md).


* * *


### Comments

* [Use this infographic as a quick reference for the client to better understand phishing](https://phishme.com/project/how-to-spot-a-phish/)

* [This EFF guide is also useful](https://ssd.eff.org/en/module/how-avoid-phishing-attacks)

