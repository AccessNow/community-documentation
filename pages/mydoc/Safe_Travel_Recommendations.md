---
title: Safe Travel Recommendations
keywords: organization security, safe travels, security policy
last_updated: April 26, 2018
tags: [organization_security, articles]
summary: "A client needs to secure their electronic devices and communications while travelling."
sidebar: mydoc_sidebar
permalink: safe_travels_recommendations.html
folder: mydoc
---


# Safe Travel Recommendations
## Basic recommendations for clients who are planning to travel and want their devices to be safe

### Problem

The client is seeking advice about how to keep their computer, phone or
information safe while travelling.


### Solution

#### Initial evaluation

We need to evaluate the situation in the country the client is travelling to, as
well as the client's needs, by asking the client the following questions:

1. Which country or countries will you visit during their travels?
2. Do you need to travel with your devices?
3. Do you need to access sensitive data while travelling?
4. Do you need to encrypt your communications?
5. Do you need to access your email and/or social media accounts?

Once we know which country or countries the client will visit, we need to answer
these questions by examining the context:

- Is the country censoring the internet?
- Does the country have a high Internet penetration rate with high speed Internet connections available?
- Are there any laws against the import or usage of encryption?
- What do the border controls imply?
    - Can the authorities force someone to unlock their devices or storage
      media?
    - Can the authorities request passwords of email and social media accounts?
    - Could the authorities seize the client's devices?


#### Recommendations

1. If the country is censoring the internet, we should recommend the usage of
circumvention tools - see ["Censorship Circumvention"](#Circumvention) below.

    If the country is not censoring the internet, we should still recommend the
    usage of a VPN for encrypting connections when the network is not secure -
    see ["Insecure networks"](#Insecure_networks) below.

2. If the import or usage of encryption is banned, the client should make sure
that no encryption software or encrypted files are present in their devices when
crossing the border. If they need to encrypt or decrypt data or communications,
they should download the software and/or the encrypted files from a cloud
through a trusted connection (see ["Data minimization and
backup"](#data-minimization) below).

    - [World map of encryption laws and
      policies](https://www.gp-digital.org/national-encryption-laws-and-policies/)
    - [Detailed crypto import/use/export information by
      country](http://cryptolaw.org/)

3. If the the authorities can force visitors to unlock their devices or storage
media at the border, the client should leave their devices at home or travel
with a barebone computer, or else minimize their data (see ["Data minimization
and backup"](#data-minimization) below).

    If the authorities can request passwords of email and social media accounts,
    the client should consider creating alternative accounts (see ["Alternative
    accounts"](#Alternative_accounts) below).

    If the authorities could seize the client's device, they should consider
    travelling without a device, as a device that is not constantly under their
    control might be compromised (see ["Leaving devices at
    home"](#Leaving_devices_at_home) below).

4. If the client needs to travel with their own devices, they should back up all
their data and leave them at home (see ["Data minimization and
backup"](#data-minimization) below). They should however think twice if there is
a high risk that their device is seized.

    If the device they need to take with them is a mobile phone, they might
    consider leaving their SIM card at home and buying a new one once they're
    inside the country.

    If the client does not need their own devices, they can consider travelling
    with an alternative laptop and/or a burner phone (see ["Leaving devices at
    home"](#Leaving_devices_at_home) below).  If the software they need is not
    illegal in the country, they can install the software they will need, but
    it's a good idea to travel with as few data as possible.

5. If the client keeps data on their devices while travelling, they should
use full-disk encryption (see ["Full-Disk encryption"](#FDE) below).

    - If encryption is illegal and/or the authorities can force the client to
      unlock their devices at the border, it is better to store their data in an
      encrypted folder in a trusted server or cloud service and download them
      through a secure connection once they're inside the country (see ["Leaving
      devices at home"](#Leaving_devices_at_home) below).
    - If encryption is not banned, but the authorities can force the client to
      unlock the devices, they can store the data in a hidden volume with
      Veracrypt (see ["Leaving devices at home"](#Leaving_devices_at_home)
      below).

6. If the client needs to encrypt their communications, we should give them the
following advice:

    - **email** - if encryption is not illegal in the destination country, they
      should store their PGP keys in an encrypted USB stick that they keep
      always with them. If encryption is illegal, they can store the keys in an
      encrypted folder in a trusted server or cloud service (see ["Leaving
      devices at home"](#Leaving_devices_at_home) below).
    - **mobile phones** - see ["Secure communications on mobile
      devices"](#secure-comms-mobile) below.
    - If encryption is illegal in the destination country, any encryption
      software should be downloaded through a trusted VPN or through Tor when
      the client is inside the country.

7. If the client needs to access their email/social media accounts, they should
activate [multi-factor authentication](#MFA) and use [strong and unique
passwords](#passwords), which they should store in an encrypted KeePassX
database.

    If encryption is banned in the destination country, the encrypted KeePassX
    database can be stored in a trusted server or cloud service and downloaded
    after the border control.

    When connecting to their accounts, the client should always check that they
    are connecting to the website through TLS/SSL and use a VPN if they're
    connecting to the web through an untrusted network (see ["Insecure
    networks"](#Insecure_networks) below).

    If the client doesn't need to access their email/social media accounts, they
    can create an alternative account for communications (see ["Alternative
    accounts"](#Alternative_accounts) below).


#### Basic security practices

Some of the following recommendations are general security practices, but they
should be implemented with special care when planning a journey.

- Check that the client's **system is updated** (operating system, programs,
  anti-virus).

- Check that an **antivirus** is installed in the client's system, otherwise
  provide them with instructions for installing it (see article #128 ["FAQ -
  Antivirus for Mac"](../Vulnerabilities_and_Malware/FAQ-Antivirus_for_Mac.md)).

    - [Avast](https://securityinabox.org/en/guide/avast/windows)
    - [AVG](https://www.avg.com/us-en/free-antivirus-download)

- Warn the client against opening **non requested attachments** or **strange
  emails**.

<a name="MFA"></a>
- Recommend to set up **multi-factor authentication**.

    - EFF's Security Self-defence guide on [setting up multi-factor
      authentication](https://ssd.eff.org/en/module/how-enable-two-factor-authentication)
    - **Google**: Please refer to article #90 [Two Steps verification for Gmail
      account](../Authentication_Security/Google_2FA.md).
    - **Outlook** and **Microsoft** [FAQ on
      2FA](http://windows.microsoft.com/en-us/windows/two-step-verification-faq)
    - **Yahoo**: Please refer to Article #168 [Secure Yahoo account with 2 step
      verification](../Authentication_Security/Yahoo_2FA.md). Also see the
      [guide by Yahoo](https://help.yahoo.com/kb/SLN5013.html)

- Warn the client against **shoulder surfers** or **cameras** that could record
  their passwords while they're entering it.

- Recommend the client to always **keep their devices with them** and to switch
  them off whenever they have to leave them unattended. They should also enable
  the **automatic screenlock** feature on all devices.
<a name="passwords"></a>
- If the client does not use **strong and unique passwords**, it is important
  that they do so before their travels.

    - [EFF's guide on strong
      passwords](https://ssd.eff.org/en/module/creating-strong-passwords)


<a name="data-minimization"></a>
#### Data minimization and backup

The client needs to understand that it is better to minimize the data they will
be carrying with them. If possible, they should travel with a barebone computer,
otherwise they should back up sensitive data and/or data that are potentially
illegal in the destination country to an encrypted device and leave them at
home.

- Please refer to article #182: [FAQ Secure
  Backup](../File_Storage_Security/Secure_Backup.md)

Potentially illegal data might include authorized copies of copyrighted material
(such as music and video), pornography, and even innocent photographs of
unclothed minors.

If they need data while travelling to a country where these data might be
illegal, they can store either just their data (encrypted) or an entire image of
their system complete with software in a trusted server or cloud service
provider and travel with a barebone laptop. Once arrived at their destination,
they can download the data and/or software, and re-upload them before departure.
This setup provides both data minimization and an accessible backup, but it
limits work while in transit.

<a name="Leaving_devices_at_home"></a>
#### Leaving devices at home

If the client does not need to take their devices with them, we should recommend
they leave them at home in a safe or in a trusted environment.

While they're travelling, they can take with them a travel laptop and/or a
burner phone. These devices should be [encrypted](#FDE) and equipped with VPN
access, and should possibly contain no information. If the client needs access
to specific files, we can set up a server where they can store encrypted files
and then download them to their computer once they are inside the country.

- If the client is going to travel with a ChromeBook, [this is a good resource
  for its preparation](https://medium.com/@seamustuohy/administering-chromebooks-e4e924907352).

Another safer way of carrying data, if it's unlikely that the authorities will
request to unlock all devices and media at the border control, and if encryption
is not illegal in the destination country, would be to store the data encrypted
in a hidden [VeraCrypt](https://veracrypt.codeplex.com/) volume in a USB stick,
or else in a Tails [encrypted persistent
volume](https://tails.boum.org/doc/first_steps/persistence/index.en.html) live
USB.

If it is advisable to travel with no devices, the client will have to rely on
shared computers.

When using shared computers, the client should avoid exchanging sensitive
communications or log into personal accounts, and if they need to do so, they
should always remember to log out of their accounts at the end of the session
(also see ["Alternative accounts"](#Alternative_accounts) below).

We should warn the client that a keylogger or other spyware may have been
installed in the shared devices they will be using. The best solutions to this
is a custom live USB that has been prepared with their choice of operating
system and the basic software they need. This lets them boot their own trusted
operating system from the USB and bypass the untrusted computer's standard setup
entirely. A good solution, can be a [Tails](https://tails.boum.org/) USB stick.


<a name="FDE"></a>
#### Full-disk encryption

**Important: If the destination country bans the import or usage encryption, we
should warn the client not to cross the border with encryption software or
encrypted data.**

Recommend to enable full-disk encryption on all the devices the client will be
carrying during their travels.

- Please refer to article #166: [FAQ - Full disk
  encryption](../File_Storage_Security/FAQ-Full_disk_encryption.md)


<a name="Insecure_networks"></a>
#### Insecure networks

It is very important that when connecting to insecure networks, for example in
hotels, airports or cafes, a VPN service is used. A compilation of VPN providers
that claim to respect users' privacy can be found
[here](https://torrentfreak.com/vpn-services-anonymous-review-2017-170304/). The
most important aspect is making sure that the provider can be trusted.


<a name="Circumvention"></a>
#### Censorship circumvention

- Please refer to Article #175: [FAQ - Circumvention & Anonymity tools
  list](../Secure_Communications/Circumvention_Anonymity_tools_list.md).

- Using Tor:
    - [General
      information](https://securityinabox.org/en/guide/torbrowser/windows)
    - [Tor on Windows](https://ssd.eff.org/en/module/how-use-tor-windows)
    - [Tor on Mac](https://ssd.eff.org/en/module/how-use-tor-mac-os-x)
    - [Tor on Linux](https://ssd.eff.org/en/module/how-use-tor-linux)

Please note that for the case of China, Kazakhstan or other locations where Tor may be
blocked, it is important to add bridges to the Tor setup (in the case of China,
have the user select meek bridges).

- Article on what to do when [Tor is blocked in a
  country](https://blog.torproject.org/blog/breaking-through-censorship-barriers-even-when-tor-blocked)
- [FAQ on Tor bridges](https://bridges.torproject.org/)
- [How to add bridges in the Tor
  Browser](https://www.torproject.org/docs/bridges#AddTorNotWorks)
- See [article on travelling to
  China](Digital_security_advice_when_traveling_to_China.md)

<a name="Alternative_accounts"></a>
#### Alternative accounts

If the client does not need to access their email and social media accounts,
they can create new accounts just for the trip that they will "throw away"
afterwards.

They can use the temporary address for all non-sensitive communications while
travelling, so that if the account is compromised it will give the attacker no
value beyond the end of their trip.

Alternative social media accounts could be useful in case the authorities can
force visitors to disclose the passwords for their accounts at the border, but
the client should be aware that a recently opened and/or inactive account might
be less credible and that they should spend some time populating the alternative
accounts with connections (possibly not their real network of friends and
colleagues) and non-sensitive content.

Recommend the client not to log into their regular accounts until or unless they
can be confident that the connection and computer are safe.


#### Mobile devices

Mobile phones should generally be considered as insecure, and it's better to
travel with a burner phone. If the client needs to take their work phone with
them, they should back up all data in a different device and remove them from
the phone and its memory card.

- [Basic general recommendations for feature
  phones](https://securityinabox.org/en/guide/mobile-phones)
- [Basic general recommendations for
  smartphones](https://securityinabox.org/en/guide/smartphones/)
- [Basic security settings for Android
  devices](https://securityinabox.org/en/guide/basic-setup/android)


<a name="secure-comms-mobile"></a>
##### Secure communications on mobile devices

Even if mobile devices are less secure than laptops, they can be useful to
establish a secure communication channel while travelling, thanks to end-to-end
encrypted messaging and voice apps like WhatsApp, Signal or Wire.

- See article #204: [Encrypted voice communications on
  mobiles](../Secure_Communications/Encrypted_voice_communications_on_mobiles.md)
- [Mail encryption on Android](https://securityinabox.org/en/guide/apg/android)
  (the client should be warned to use a subkey or to generate a different pair
  of keys for using GPG on a phone)


### Comments

**Make sure the links are working properly before sending to the client.**

#### Resources

- A post on the Access Now blog with [general guidelines on digital security
  while
  traveling](https://www.accessnow.org/blog/2015/03/17/best-practices-for-digital-security-while-traveling-to-rightscon)
- EFF published a [travel guide focused on US border
  crossing](https://ssd.eff.org/en/module/things-consider-when-crossing-us-border)
- [Establish a technical and legal shield against the latest laptop ban
  concerning certain
  airlines](https://www.eff.org/wp/digital-privacy-us-border-2017)
- [Princeton University International Travel guide](
  https://informationsecurity.princeton.edu/intltravel)
- The [Umbrella app](https://secfirst.org/index.html) offers important tips on
  safer travels for people at risk
