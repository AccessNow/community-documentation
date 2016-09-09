---
title: Tor Exit Node Abuse Complaint 
tags: [article, procedures, tor-abuse]
keywords: tor, stalking, harassment, abuse, tor exit node, exit node, exit, tor abuse, tor node, complaint, hacking, tor hacking, tor complaint, TOR, Tor
summary: Someone detected abuse from an IP address.
sidebar: mydoc_sidebar
permalink: mydoc_tor_abuse.html
folder: mydoc
---


#### Problem   
1. The IP address is one of our Exit Node Addresses.
2. Is the complainer a human being or a bot?

#### Solution  
1. Check if the IP address is one of our exit node addresses

   For more details about the IPs: https://www.dan.me.uk/tornodes

2. You should immediately log into the Tor Exit node in question, and perform basic checks to ensure that the box has not been hacked and compromised. 

   * First, ssh into the suspicious machine.
   > ssh [remote_username]@[remote_host] -p [port_number]

   * Then, use the following commands in your investigation:

   |Command|What It Does|
   |-------|------------|
   | > last | displays a list of users that have logged in and out |
   | > who | displays who is logged on currently |
   | > ps auwx | <ul><li>ps: displays current processes</li><li>a: displays processes for all users</li><li>u: displays process belonging to specified user</li><li>w: use 132 columns to display information, instead of default window size</li><li>x: display processes not attached to a terminal</li></ul> | 
   | > lsof | lists open files (think ls + of) |

   * Look at recent activity in the logs, particularly auth.log, syslog, daemon.log

3. If the node is determined "not compromised", then the next step is to send our standard response to the address we received the email from. The exact emailed response depends on the risk and impact of each particular abuse case.

   * In high risk cases, when someone's physical security is being threatened or a non computer-related crime is being committed through our exit node, use the ["Tor Abuse - Threatening Harassment"](#threatening) template.

   * In low risk cases, if the received complaint is related to a network scan, illegal access attempt, spam, forum/groups spam, MySQL injections, Cross-Site Scripting, Cross-Frame Scripting, DoS attacks and so on, use the ["Tor Abuse - Non-threatening Harassment"](#nonthreatening) template.

4. If we receive a second response, then we can engage in a discussion with them and ensure they understand what is going on. We can let them know that if attacks from Tor Exit nodes are a serious problem they should consider automating the process of downloading the lists of Exit nodes from the Tor Project, and block access to their resources from those Tor Exit nodes.

5. After we send the initial response (see step 3), wait for one week for a reply. If we do not hear back, send a follow up email. We can use the [Tor Abuse - Follow Up](#followUp) template.

6. After the follow up is sent, wait another week. If there is still no response from a human, then close the case.

#### Comments:   
- Please use "Successfully Solved" when the case is closed, regardless of whether the claimant responded or not.
- Please DO NOT MERGE complaints cases, even if we get multiple complaints from the same organization or person. Each instance of an attack / complaint should be treated as a separate case.
- If the complaints are coming from an automated system then the process is to ask to speak to a human to explain the situation



## Templates for Tor Exit Node Abuse Cases

### <a name="threatening"></a>Template - Tor Abuse - Threatening Harassment

Dear $CLIENT_NAME,

My name is $HANDLER_NAME, and I am part of the Access Now Digital Security Helpline. I am very sorry to hear about your situation. I understand how difficult an experience this is, and I know it may be hard to figure out the next step to take.

If your physical security has been threatened, please consider contacting law enforcement, or creating a log of the abuse. A paper trail may seem useless now, but it creates considerable proof of harassment for later.

Unfortunately, the IP address you reported is associated with a Tor Exit Node (also called an open relay). This means that the abuser is not using our node specifically, but the Tor network as a whole. 

The Tor Project is designed to provide anonymity to its users. Its structure makes it impossible for us to find the real perpetrator of the abuse online. This does not mean that nothing can be done -- traditional investigative techniques are still very effective -- but it does mean the Helpline won't be in a position to help.

Please let me know if I can be of further assistance. Once again, I am very sorry to hear of your situation, and I hope you are able to resolve it safely soon.

To find out more about how to protect yourself on and offline, read:
* https://yaelwrites.com/saferonline.pdf

For more information on Tor, please visit  
* https://www.eff.org/torchallenge/what-is-tor.html 
* https://torproject.org

Regards,
$HANDLER_NAME



### <a name="nonthreatening"></a>Template - Tor Abuse - Non-threatening Harassment

Dear $CLIENT_NAME,
    
My name is $HANDLER_NAME, and I am part of the Access Now Digital Security Helpline. I am very sorry to hear about your situation. 

Unfortunately, the IP address you reported is associated with a Tor Exit Node (also called an open relay). This means that the abuser is not using our node specifically, but the Tor network as a whole. 

The Tor Project is designed to provide anonymity to its users. Its structure makes it impossible for us to find the real perpetrator of the abuse online. Connections are routed through multiple relays, and multiplexed together between. The system does not record logs of client connections or previous hops.

I can offer to block specific destination IPs and ports, but the abuser doesn't exclusively use our relays; he or she will just be routed through a different exit node outside of our control instead.

I'm very sorry for the inconvenience. Please let me know if I can be of further assistance. 

If you would like more information about Tor, please visit  
* https://www.eff.org/torchallenge/what-is-tor.html 
* https://torproject.org

Regards,
$HANDLER_NAME



### <a name="followUp"></a>Template - Tor Abuse - Follow Up 

Dear $CLIENT_NAME,

Unfortunately, as explained in the previous email, the server involved is a Tor exit relay and the abuser is not exclusively using this server, but the whole of the global Tor network. 

The best we can offer is to block specific destination IPs and ports, but he/she will just be routed through a different exit node outside of our control instead.

If you have any additional questions, please don't hesitate to contact me. I'm sorry we cannot be of more assistance.

Regards,
$HANDLER_NAME