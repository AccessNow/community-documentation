---
title: FAQ - Secure Backup
tags: [article, support, security-assessment]
keywords: backup, file storage security
summary: Backup policy and process for different types of devices (laptops and smartphones), Windows, Linux, Mac OS X, Android, iOS
sidebar: mydoc_sidebar
permalink: mydoc_secure_backup.md
folder: mydoc
---


# FAQ - Secure Backup
## Backup policy and process for different types of devices (laptops and smartphones), Windows, Linux, Mac OS X, Android, iOS

### Problem

- The client's data are already lost.
- There's a risk of loosing data due to the device/s being seized.
- The client would like to learn how to back up data in a secure way.
- The client is traveling to a sensitive country.
- The client needs to develop a disaster recovery plan.


### Solution

It is always recommended to back up the data in our device/s, especially if they are  sensitive and important. However, before proceeding with the backup process, we need to take precautions to ensure a secure backup.

Before deciding on a backup and recovery strategy, we have to ask the following questions:

- **Why?** - Why are you protecting yourself against disaster? Does it matter if you lose data? What losses will you suffer (in terms of money, etc.)?
- **What?** - What are you going to back up? Your entire hard drive or just some of the data?
- **When?** - When is the best time to back up your system? How often will you perform a backup? When will you use full backups and incremental backups? We urge everyone to carry out regular backups.
- **Where?** - Where will the backups be stored? On-site? Off-Site? In a cloud (Dropbox, Google Drive, SkyDrive, etc.)? Where is our important information actually (computer hard drive, USB / external drive, cloud storage, smartphone, etc.)?
- **Which Medium?** - Attached storage (USB stick, USB hard drive, tape drive), backup server?

After gathering all the necessary information from the client, we need to clarifywith them that there is a possibility of data loss. One common disaster scenario occurs when only duplicates of an important document are backed up, and the master copy itself (the most up-to-date version of a particular file or collection of files) gets lost or destroyed before those duplicates can be updated. 

For each backup support, an online backup service (backup server, Cloud, etc.) or an external hard drive (USB, external drive, etc.), we highly recommend to encrypt files/folders before uploading them. For the external hard drive, FDE in advance would be good.

In case the client is planning to travel, we need to recommend to never carry both their laptop and backup hard drive at the same time.

There are many tools that could be used to encrypt files, depending on the operating system of the device:


#### Online Backup Service


- **Advantage**: Data has high availability with internet connection.
- **Inconvenient**: These services are usually third-party commercial cloud services, like Dropbox, oneDrive, or iCloud, which have full control over our stored data on their servers. We don't have a guarantee that our data are private and the service owner has not access to them.


#### External Data Storage Device

- **Advantage**: You have full control of all backed up data, and you can encrypt your hard drive with any tools you prefer or you are familiar with. 
- **Inconvenient**: This device could be seized or stolen, we could not have access to the contents of the drive remotely. 

##### For Windows

- **Cobian Backup** is used for creating archives of your digital files. They can be stored on your computer, office network, removable devices or Internet servers.

    For more details, please visit [this link](https://securityinabox.org/en/guide/cobian/windows/)

##### For OS X

1. Encrypt files with GPG, based on the article ["Encrypt files on a Mac thanks to GpgTools"](Encrypt_files_Mac_GpgTools.md).
2. Back up with [Time Machine](https://support.apple.com/kb/PH18835?locale=en_US).

##### For Android

- **Manual backup** - We could connect an Android phone to a laptop (better if this has full-disk encryption), and then transfer all selected files.

    If the client has a Mac OS laptop, they need to install Android File Transfer for Mac. For more details, visit [this link](https://www.android.com/filetransfer/)

- **Remote automated** - In addition, Android haw a backup option which lets you back up some data in the phone on your Gmail account.
    1. The *Account and sync* feature can back up contacts, Gmail, Picasa Web Album and Calendar. The data are synced in the user's Google account.
    2. The *Back up my data* option lets you save a wide variety of your personal data, including Wi-Fi passwords, browser bookmarks, a list of the apps you’ve installed on Google Play, the words you’ve added to the dictionary used by the onscreen keyboard, and most of your customized settings. The whole process is automatic. 

        For more details visit [this link](https://support.google.com/nexus/answer/2819582?hl=en)

- **DropBox backup** - *Cryptonite* is a free and open source file encryption solution based on the original EncFS code. It lets you encrypt files before you upload them to Dropbox. Mounting doesn't work on some Android 4.2 devices. 

Please visit [this link to download the tool](https://play.google.com/store/apps/details?id=csh.cryptonite)

##### For iOS

- **iTunes** has an option to backup the iOS device onto a computer. By selecting the “Encrypt backup” option in the Summary tab of your device in iTunes, iTunes will back up more confidential information (such as Wi-Fi passwords and email passwords), but will encrypt it all before saving it onto the computer.

- **Apple's iCloud** is another option, less recommended than the iTunes one. The client should use a long passphrase to protect the data, and keep that passphrase safe. While Apple encrypts most data in its backups, it may be possible for the company to obtain access for law enforcement purposes (especially email and notes, which at the time of writing are stored unencrypted).

*Note:* If the data protection is turned on, it will also be able to delete the data on the device securely and quickly. In the Passcode settings, the client can set their device to wipe all its data after ten failed attempts to guess the passphrase.


##### For Ubuntu

- **Rsync**  is a protocol built for Unix-like systems that provides versatility for backing up and synchronizing data. It can be used locally to back up files to different directories or can be configured to sync across the Internet to other hosts.

    Instructions on how to use Rsync to back up data can be found [here](http://www.cyberciti.biz/tips/linux-use-rsync-transfer-mirror-files-directories.html)

    More backup solutions are listed [in this page](https://help.ubuntu.com/community/BackupYourSystem)


### Comments

There are different backup methods:

- **Manual** - Manual backup is initiated on a schedule by the user and is the most common method for home users to back up their files. This method is also the least reliable.

- **Local automated** - Automated backups that target a hard drive or tape drive attached to the physical box being backed up fall into this category. Advanced home users and small businesses will often use this method.

- **Remote automated** - Automated backups that target a hard drive, tape drive or virtual tape library (VTL) over the network fall into this backup method. This type of backup is often used by businesses that have money they can dedicate to the process of backup. As the organization becomes more mature, they may even stage the backup on multiple mediums and increase the distance between backup and production systems.

#### Some useful links:

- [Level Up's Data Backup Basics](http://www.level-up.cc/curriculum/protecting-data/data-backup-basics/)

- [Security in a Box - Tactics on Backup](https://securityinabox.org/en/guide/backup)
