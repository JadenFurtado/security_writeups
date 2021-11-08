

# ARP poisoning

## Introduction:
Just a writeup on ARP poisoning, based on everything that I know and have studied about the Address Resolution Protocol (ARP) to help me retain my knowledge.

## What is ARP?
ARP is short for address resolution protocol. It is generally used by the IPv4 protocol. As the name suggests, it is used to convert the IP address of a machine to it's MAC address. 
![alt text](https://cdn.slidesharecdn.com/ss_thumbnails/addressresolutionprotocol-121115085659-phpapp01-thumbnail-4.jpg?cb=1352969854)

This protocol operates in the Data Link layer of the OSI model.
![alt text](https://media.geeksforgeeks.org/wp-content/uploads/computer-network-osi-model-layers.png)

In theory, an ARP should:

Accept requests. A new device asks to join the local area network (LAN), providing an IP address. 
Translate. Devices on the LAN don't communicate via IP address. The ARP translates the IP address to a MAC address. 
Send requests. If the ARP doesn't know the MAC address to use for an IP address, it sends an ARP packet request, which queries other machines on the network to get what's missing. 
This functionality saves network administrators a lot of time. Requests are handled behind the scenes, and the network does all the cleanup required.

## What is ARP poisoning and ARP spoofing?
A malicious developer, hoping to gain access to important data, could expose vulnerabilities and sneak inside, and you may never know it's happening. 

Two types of ARP attacks exist.

- ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
- ARP poisoning: After a successful ARP spoofing, a hacker changes the company's ARP table, so it contains falsified MAC maps. The contagion spreads.

![alt_text](https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/ARP_Spoofing.svg/1200px-ARP_Spoofing.svg.png)

The goal is to link a hacker's MAC with the LAN. The result means any traffic sent to the compromised LAN will head to the attacker instead. Effectively this is like a man in the middle attack.

## What can a successful APR poisoning result in?

- Hijack:
Someone may look over everything that heads to the LAN before releasing it. 
- Deny service:
Someone may refuse to release anything from the infected LAN unless some kind of ransom is paid. 
- Man in the middle:
Someone conducting a man-in-the-middle attack can do almost anything, including altering documents before sending them out. These attacks both threaten confidentiality and reduce user confidence. They are among the most dangerous attacks anyone can perpetrate. 
If a hacker wants to take over an end host, the work must be done quickly. ARP processes expire within about 60 seconds. But on a network, requests can linger for up to 4 hours. That leaves plenty of time for a hacker to both contemplate and execute an attack.

### Reference:

- https://www.okta.com/identity-101/arp-poisoning/

### Credits:
- SlideShare for the APR diagram
- Geeks for geeks for the OSI datagtam image
