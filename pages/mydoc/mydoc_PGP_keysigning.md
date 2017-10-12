---
title: PGP key signing
tags: [article, support, email_security]
keywords: PGP, email security, web of trust
summary: How to sign a PGP public key to enhance the web of trust and/or address a key tampering attack 
sidebar: mydoc_sidebar
permalink: mydoc_PGP_keysigning.html
folder: mydoc
---


# PGP key signing
## How to sign a PGP public key to enhance the web of trust and/or address a key tampering attack 

### Problem

- A new team member is being onboarded and a new key is being generated for them;
- A client has been targeted with a PGP key tampering attack (additional
  non-revoked public keys have been created and uploaded to the keyservers
  without their knowledge)

In both cases, we need to enhance the web of trust for a PGP key to help confirm
that the PGP key belongs to a legitimate user and is connected to their email
address.


### Solution

Once PGP has been set up for the client/new team member and we have a copy of
the public key, if the below requirements are met, we can proceed to verify and
sign it. The action of signing someone's public key should be done very
carefully, so before signing a key, we need to verify that the key we are
signing is actually connected to the client’s/new team member’s email, and that
the owner of the key is also the legitimate owner of the connected email
account. The following steps are required for the verification:

- The client has been vetted and is a member of civil society
- We have met the key owner in person, or at least in video-chat
- We have proof that the key owner is the legitimate owner of the connected
  email account, for example because an intermediary can vouch for them, or we
  have asked them to reply to our email
- We have checked the fingerprint of the key we want to sign corresponds to the
  fingerprint of the user’s key
- If we are replying to an incident, we should check if the client has been
  targeted by a key tampering attack

If the verification is successful, we can proceed to sign the key and inform the
client/new staff member that we are going to sign their key.

1. If the client is willing to upload their PGP key to the keyservers, we can
proceed to sign the key. Once we have signed it, we can send the client/new staff
member his/her signed public key and instruct them on how to publish it on the
keyserver.
2. If the client would rather not publish their PGP key, we can sign their key
locally, so that they cannot be exported (but this won't help address a key 
tampering attack).

**If the verification is not possible or successful, we should not sign their PGP key.**

**Keys should always be signed with the incident handler’s personal key.**


### Comments

- We should not directly upload the signed key to the keyservers.
- We should warn the client about the risks of having their key signed by a
  member of the   Digital Security Helpline, as this will disclose a connection
  between them and the Helpline, and also of publishing their PGP public key to 
  the keyservers in the first place, as this can expose the fact that they are 
  using encryption.
- Once the client/new staff member has uploaded their key to the keyservers, we
  should check if our signature has been reflected in the public key, else we
  should get back to the client and offer assistance.
- If a Helpline team member has already signed the key, we can skip the
  verification process and sign the key.