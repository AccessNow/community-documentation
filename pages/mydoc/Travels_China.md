---
title: Digital security advice when travelling to China
keywords: organization security, safe travels, security policy, China, travels
last_updated: April 26, 2018
tags: [organization_security, articles]
summary: "A client who is preparing a trip to Mainland China has asked us for advice."
sidebar: mydoc_sidebar
permalink: travels_china.html
folder: mydoc
---


# Digital security advice when travelling to China
## Best practices and precautions for clients who are travelling to Mainland China

### Problem

A client is preparing a trip to Mainland China and needs to prepare a digital security policy to protect their activities while travelling in the country.


* * *


### Solution

#### Information Gathering

- Find out if the client is a Chinese national or not - for Chinese nationals
these recommendations might be problematic and we might need to consult with 
trusted partners. It is also important to know what kind of visa they will be
travelling with, as some visa (for example a journalist visa) expose to a 
heightened level of surveillance.

- Ask if they must take their own devices (laptops or smartphone) or if it is
possible to use devices especially set up for this trip. We should try to encourage the usage of travel devices, as the risk of a device being infected with malware or being confiscated is high. Based on this answer, [case 1](#case1) or [case 2](#case2) will be recommended.


**Other questions we should ask the client:**

- What is the purpose of the trip?
- What are the client’s needs during the trip? (For example, do they need to receive sensitive information via email, video chat or chat? Do they need access to encrypted emails? Do they need to conceal their identity? etc.)
- Can the client travel without any devices, or must they absolutely bring devices with them? What devices must they take? 
- Will they be carrying sensitive information when leaving the country?
- If they are planning to carry out sensitive activities or are going to handle sensitive materials, we should also check that the client has an operations security strategy in place for travelling in Mainland China. For example, how are they going to explain their travels to the authorities? Do they have trusted contacts in China? How will they describe their work to local people? 


#### Basic digital security review checklist

**For general recommendations on safer travels, see [article #181 on safer travels](Safe_Travel_Recommendations.md)**

1. Is two-factor authentication enabled for their email and social media accounts?

    If 2FA is enabled, ensure they are using app-based 2FA or a security key, and not SMS-based 2FA. Ensure they bring the phone or security key with them or have printed 2FA backup codes. 

2. Is device encryption enabled for their devices?

    The client should enable full-disk encryption, but we should also warn them that they might be required by the authorities to give them the passphrase to decrypt the device. They should be prepared to handle inspections, and decide in advance if they prefer to give them the passphrase. They should also make sure that if the authorities cannot gain access to their devices, and decide to take serious measures like detention, they have a contingency plan in place, possibly including  trusted local contacts.

    Once we have made sure that full-disk encryption is enabled in their devices, we should ensure they understand that the device is fully encrypted only when it is off, and that they have a strong passphrase for it (as well as screen lock enabled). Warn them of the risks and concerns associated with device encryption as described below:

    The client should understand that when crossing the border the authorities may ask for the passphrase to decrypt the device.

    The encrypted data is only protected when the computer is off. If an adversary gets access to the computer while it’s on, in sleep mode, or hibernated, there are several techniques that can be used to extract data.

    Encryption is only as good as the encryption password. If the attacker has the user's device, they have all the time in the world to try out new passwords.
While encryption can prevent casual access, the client could be forced to reveal their passphrase, so they should preserve truly confidential data by not having it on the device itself. There are also strategies for hiding data to reduce the likelihood of any physical access. The client should not trust their encrypted machine implicitly.

    Additional information on full-disk encryption can be found in [article #166: FAQ - Full Disk Encryption FDE](Devices_Data_Security/Full-Disk_Encryption.md).

3. Do they have a device backup? If so, ensure they understand the importance of keeping it in a safe place, possibly at home, separate from their device and encrypted.

    Refer to [Article #182: FAQ - Secure Backup](../Devices_Data_Security/Secure_Backup.md) for further information on secure backup.

4. Do they have circumvention tools installed in the devices they will travel with? 

    All the devices should have more than one circumvention tool installed and set up prior to travelling in case some of them don't work in the country.
refer to [https://cc.greatfire.org/en](https://cc.greatfire.org/en) to verify available and functional VPN services in China.

    - See [article #175: FAQ - Circumvention & Anonimity tools list](../Anonymity_Circumvention/Circumvention_Anonymity_tools_list.md)
    - See [article #110: How to circumvent the Great Firewall block in China](../Anonymity_Circumvention/VPN_China.md)


#### Specific recommendations

<a name="case1"></a>
##### Case 1

The client accepts to use a different device especially set up for the trip (a travel laptop and/or a smartphone).

The device will be encrypted and equipped with VPN access among other security measures, and it won’t contain any information on the hard drive. If the client needs access to specific files, we can set up a place to download encrypted files to their system once they are in the country.

If the client is going to travel with a ChromeBook, [this is a good resource for its preparation](https://medium.com/@seamustuohy/administering-chromebooks-e4e924907352).

<a name="case2"></a>
##### Case 2

The client requires to take their own devices. In this case, safe travel recommendation should be sent to them according to their context and needs,
following [art. #250, a template with a setup checklist](../Templates/China_travels_checklist.md).

**NOTE:** advise the client to download the applications they need before travelling to China, or else verify if the website to download the tools is available in China by checking [this website](https://en.greatfire.org/analyzer).


* * *

### Comments

It's important that we always follow up with the client after their travels:
since information on digital security in China is scarce, getting their feedback
on our recommendations can improve our knowledge of the ongoing development in
the country.


#### Additional Resources


- [A Digital Security Guide for countries at risk](http://practicaldigitalprotection.com/#en ) - the English version is a translation from the version for China. Much of this guide is based on personal experience.

- Reading this story would also be good preparation for any trip to China where you may be carrying or obtaining sensitive materials or dealing with sensitive matters.

