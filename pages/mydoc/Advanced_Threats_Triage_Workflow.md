---
title: Advanced Threats Triage Workflow
keywords: vulnerabilities, malware, triage, advanced threats, APT, advanced threats
last_updated: April 26, 2018
tags: [vulnerabilities_malware, articles, faq]
summary: "The client has received suspicious messages, or suspicious behaviour has been observed in the client's devices or network."
sidebar: mydoc_sidebar
permalink: advanced_threats_triage_workflow.html
folder: mydoc
---


# Advanced Threats Triage Workflow
## Rapid Response Workflow for Advanced Threats

### Problem

- Suspicious behaviors, processes, traffic, or other "weird activities" have been found in the client's devices or network.
- The client has received phishing or suspicious emails that seem targeted.

Some of these suspicious activities might be false positives related to other non-malicious software causing the machine to act weird or (most commonly) other types of less serious (and non-targeted) malicious software like adware. When this cannot be ruled out, collecting evidence, running basic analysis, and assessing the risk and impact against organizational priorities will help prioritize further action.


* * *


### Solution

#### Preparation

* When dealing with advanced threats, we should be able to handle and capture data correctly - see [Article #252: Forensic Handling of Data](../Forensics/Forensic_Handling_Data.md).


#### Guiding Questions

* Does the organization suspect they are infected with malware? If so, what evidence supports that?
* Have staff members received suspicious communications, like emails or IMs?
* Based on the context research and the organization's activities, how likely are targeted attacks?
* How much time should be devoted to more complete analysis, and what other factors change that?
* What are the implications of targeted malware for the organization, and for the current assessment process?
* What types of malware should trigger an incident response approach?


#### Workflow

**Look for indicators of compromise**

In the following steps you should look for files and URLs that may indicate a compromise and may help you identify an infection.


##### 0. email / messages / communications

*Also see [Article #58: Client Receives a Suspicious/Phishing Email](/Phishing_Suspicious_Email/Suspicious_Phishing_Email.md).*

If the organization staff has received suspicious communications, the first step should be to clearly warn the client that any associated files or links *should not be opened*.

1. Ask the client to share the complete email with you. Instructions on how to share the complete email, which includes full headers and attachments can be found [here](https://www.circl.lu/pub/tr-34/) (this is preferred over just [asking for the headers](https://www.circl.lu/pub/tr-07/), since it is just as complicated from the user prospective but provides more information to us or a malware researcher).

2. Investigate the intent of the message. If this email appears to be spam, you can rule out an advanced threat and include in your recommendations instructions on how to report spam or mark email messages as junk.

3. If the message does not seem to be spam and has links or files attached to the email, capture any suspicious URL and save the file in an empty storage device for further analysis.

4. If the email does not have links or files and is not spam, investigate it as a potential social engineering email.

##### 1. Network scanning and traffic analysis

Advanced threats may be identified through network scanning and traffic analysis of the organization's internal network.

- For remote scanning see [this SAFETAG exercise](https://github.com/SAFETAG/SAFETAG/tree/master/en/exercises/remote_network_device_assessment)

- For network scanning see [this SAFETAG exercise](https://github.com/SAFETAG/SAFETAG/tree/master/en/exercises/network_scanning)
- For traffic analysis see [this SAFETAG exercise](https://github.com/SAFETAG/SAFETAG/tree/master/en/exercises/traffic_analysis)


##### 2. Analyze suspicious processes on individual devices

If we find suspicious open ports, we can follow the instructions in section "How to decide if an open port is suspicious" of the [SAFETAG exercise on network scanning](https://github.com/SAFETAG/SAFETAG/tree/master/en/exercises/network_scanning),

It can also be useful to follow these steps:

- On every operating system, check if the device OS and the installed software are up-to-date.

###### Windows, Mac, Android

1. Check that antivirus is installed in the device. 

    1. Check that the installed antivirus is up-to-date.
        - if an antivirus is installed, and it is up-to-date, launch a scan - this will help as a diagnostic tool, to identify any malware, not necessarily to remove it.
        - if malware is identified:
            - for commercial, known malware - get rid of it through the antivirus.

    2. If the the antivirus is disabled:
        - Try to understand if the user disabled it, and why.
            - if the user hasn't disabled it, a computer compromise is likely.


###### Android, iOS

- Check if the device is rooted or jailbroken - this might be an indicator of compromise.

    - Check if any suspicious applications have been installed from outside the official app stores.


##### 3. Analyze suspicious files

Even if we have limited time for this step, a preliminary analysis (not longer than one hour) can be performed, following these instructions:

1. Get a hash of the file and a timestamp of the event.

    1. send the hash to MISP
        - Check if there are any related events
        - Find any connected IP addresses

    2. Send the hash to VirusTotal (**Warning** - if the file is targeted malware, this might show the attacker that you're carrying out an investigation on the incident).
        - Check if the file is known.

If the file is malicious, copy it onto an empty drive for further analysis.

Remember to include the hashes of the malicious files in the appendix of your assessment report.


##### 4. Analyze suspicious URLs

You may have found suspicious URLs in your wireshark output during the traffic analysis, in the email content, in IMs, etc.

Capture the context in which the URL was sent to the user or used by a process (sender, timestamp including timezone, and any other identifying details.)

If the URL was sent to the user through a message, ask them if they clicked the link.

1. check the URL in MISP
2. open the URL in a private cuckoo sandbox instance for a forensic capture of anything malicious
3. submit the URL to VirusTotal (**Warning** - if the file is targeted malware, this might show the attacker that you're carrying out an investigation on the incident).
4. submit the URL to archive.org or archive.is for public archiving (this could also disclose your investigation to the attacker)


##### 5. Urgent incident response

*If time for this step is limited, we should at least coordinate the response with third parties, rather than carry it out ourselves.*

Some of the mitigation steps can be implemented by the user, following the instructions included [here](https://rarenet.github.io/DFAK/en/Malware/).

You should consider a compromise serious and coordinate an incident response if any of the following is happening:
    
* files are being leaked
* a keylogger or spyware has been detected in a device
* the infected device is critical for the organization

Possible mitigation steps:

- if the device is not critical, suggest the client to avoid using the infected device until a thorough investigation has been completed
- help the client delete the hard disk content and reinstall the system
- if the forensic capture of the whole hard disk would take too long, and an investigation is needed, we can suggest the client to replace the hard disk
- if reinstalling the system is not possible, the device should be replaced
- mobile devices can be reset to factory settings
    - after resetting to factory settings, we should make sure any app or data recovery is not including potential compromise vectors, such as browser extensions, malicious applications, etc.


##### Outputs

The main outputs of advanced threats identification should be evidence like files, emails, screenshots and URLs included in messages or spotted in suspicious connections.

* Identification and initial triage/analysis of suspicious processes, files, and emails (via Anti-Virus scanning results, MISP and VirusTotal information, network traffic analysis, and other research)
* Useful evidence for further analysis (including hard disk image, memory image, suspicious files, emails, network traffic captures, URLs) - see [Article #252: Forensic Handling of Data](../Forensics/Forensic_Handling_Data.md).


* * *


### Comments

#### Operational Security

* An agreement on capturing data in infected devices should be signed with the organization before this step.
* We should ensure that we have a clear understanding set with the organization on an incidence response plan, points of contact, and process to allow for safe discussions.
* Dealing with malicious software is risky, we have to be aware of the threats around it, don’t infect ourselves or more machines.
* Don't upload files to third-party services (use hashes). Take extreme care with identifying or potentially targeted information.
* Use VPNs or Tor to search if conducting the search from a country that is highly competitive with the organization’s country, or is known to surveil.

