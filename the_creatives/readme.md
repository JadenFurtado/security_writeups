# HHHHH management 

The time I hacked a modelling agency. In all fairness, I tried my best to get the attention of the agencies involved here as well as people I knew who work for/with them.(well, I knew just one person really, if you know, you know) 
Only when they did not respond to my mails/messages and all other options that I tried failed, I decided to go ahead and exploit the vulnerabilities to get it to their attention so as to fix the flaws.

## Basic gist of the hack:
The website used an API to display images of the models. However, the inputs were not sanitized and this allowed me inject SQL into the website. I was able to extract the usernames and passwords from the database. The passwords were hased using the Md5 algorithm. I was able to reverse the hash using a rainbow table and log in as admin. 

### The admin panel:

<img src="https://github.com/JadenFurtado/security_writeups/blob/main/the_creatives/admin.jpg" style="-webkit-filter: blur(4px); filter: blur(4px); "/>

### Ofcource, these are now fixed and Md5 is no longer being used!

## Full writeup : https://github.com/JadenFurtado/security_writeups/blob/main/the_creatives/Case%20Study-edit.pdf

### However, this is not all. I have not included this section in the writeup. Bit of a rant coming up!

Though the API endpoints are now being sanitized, and an SQL injection is no longer possible, the site as a whole is still insecure. There are still vulnerabilities(I have not included these in the writeup) that have not been fixed till date. I have been begging them to fix the issues for well over 2 years now (It goes way back to 2019. I did not even ask for something silly like money/bug-bounty or a hall of fame, btw! I openly and responsibly disclosed all the vulnerabilities I found and they didn't have the decency to respond to me, or acknowledge my mails even once) and so, if anyone from HHHHHHH is reading this, fix your website and reply to mails!

## Timeline

### Feb 2019 SQL Vulnerability is found and HHHHHH as well as AAAAAA is informed, but no reply to my mails or insta messages
### 6th Nov 2019, Since I got no response from HHHHHH or AAAAA, I decided to get the attention of a mutual contact and try and get her to communicate to HHHHHHH for me. Does not work
### 23rd Jan 2021, I decide to revisit HHHHHH, vulnerabilities still not fixed and an XSS vulnerability is discovered. HHHHHH and AAAAAA are informed, AAAAA finally replies that they will check my messages out but does nothing
### 8th Feb 2021, while poking about the site, I end up getting username and password and login as admin
### 10th Feb 2021, HHHHHH is informed again, this time with the new findings. They finally fix the vulnerabilities, but again don't respond to my mails!
### 9th Dec 2021, one last push from my side to get the fact of existing critical vulnerabilities across before I permanently shelve this. It does not work, and so, I will no longer be putting any more effort and time into this. 
## -----------THE-END----------

