# The Medical Company

I had absolutely nothing to do and so I put it on my Instagram story as to what you’ll would like me to do, whether to build something or hack something. You’ll chose hacking and 
so I decided to go ahead and hack. I found a company having a website with a good vulnerability disclosure program, no payments to the researcher, 
but hey, I am not interested in money. I am just doing this for fun.   

## Gist of what I did:

I found a possible SSRF vulnerability, the scope of which I am unaware of. I then tried to scan the server of the company using NMAP. 
I then saw that they had not closed off a lot of the ports and so I decided to try and brute force the SSH login of the server using Metasploit. 

### A screenshot of the open ports 

<img src="https://github.com/JadenFurtado/security_writeups/blob/main/the%20medical%20company/cmd.png" />

I happened to trip a security alarm while snooping around in their server, and well, things happened.... 

## Full writeup : https://github.com/JadenFurtado/security_writeups/blob/main/the%20medical%20company/case%20study_3.pdf

## timeline:

### 5th May 2021: Picked a target and decided to hack
### 2nd June 2021: Posted what you'll want me to do, build or hack, hacking it is!
### some time later in June 2021: Bruteforced SSH and ended up tripping an alarm and intrusion detected
### Unbanned from the website and my intrusion is cleared from their networks
