---
title: Sending signed PGP key
keywords: templates, secure communications, PGP, GPG, keysigning, web of trust
last_updated: April 26, 2018
tags: [templates]
summary: "Template to be used after signing a PGP key to send the signed key and instructions to the user."
sidebar: mydoc_sidebar
permalink: pgp_keysigning_final.html
folder: mydoc
---


# Sending signed PGP key
## Template to send a signed PGP key to a user

### Body

Dear xxxxx,

I hope you are doing great.

As we discussed in our latest exchange, I have signed your PGP key “[Client public key fingerprint]” with my own key “[your key fingerprint]”, and you can find the signed key attached here.

Now all you need to do is update your public key and upload it to the keyservers.

If you are using Thunderbird with Enigmail, these are the steps you need to follow:

- Save the attached file with your signed public key to your computer
- Open your Enigmail key manager by clicking on the settings icon in Thunderbird and then selecting “Enigmail” -> “Key Management” in the dropdown menus
- Click “File” -> “Import Keys from File”
- Select the file with your signed public key you have just downloaded and click on “Open” to import your signed key. This will update your current public key, adding my signature to your keyring
- In the Key Management window, right-click your PGP key and select “Upload Public Keys to Keyserver”. This will publish your public key on the key servers, or update it with the new signature if it was already online.

If you use a different system to manage your PGP keys and don’t know how to do this, please let us know and we will guide you through the necessary steps for your system.

Please note that before uploading your public key to a keyserver, it is a good idea to take a moment to consider whether you want the whole world to know that you are using an encryption key, without the ability to remove this information at a later time.
Even if you have no problem with your key being publicly available in the keyservers, please consider that once you update your key with my signature and upload it, your connection with the Access Now Digital Security Helpline will become public, so please ask yourself if this could entail any risks before you update your key with the new signature.

Please, don't hesitate to get in touch if you have any doubts on this process or need more explanations.

Kind Regards,
XXXXX
