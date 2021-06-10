# Anima Creatives management

The time I hacked a modelling agency. In all fairness, I tried my best to get the attention of the agencies involved here as well as people(she was just one person, really, if you know, you know. It was hilarious, LOL 😆😅😂😭😬) I knew who work for/with them. 
Only when they did not respond to my mails/messages and all other options that I tried failed, I decided to go ahead and exploit the vulnerabilities to get it to their attention so as to fix the flaws.

## Basic gist of the hack:
The website used a REST API to display images of the models. However, the inputs were not sanitized and this allowed me inject SQL into the website. I was able to extract the usernames and passwords from the database. The passwords were hased using the Md5 algorithm. I was able to reverse the hash using a rainbow table and log in as admin. 

### The admin panel:

<img src="https://github.com/JadenFurtado/security_writeups/blob/main/anima_creatives/admin.jpg" />

### Ofcource, these are now fixed and Md5 is no longer being used!

## Full writeup : https://github.com/JadenFurtado/security_writeups/blob/main/anima_creatives/anima_case_study.pdf

### However, this is not all. I have not included this section in the writeup. Bit of a rant coming up!

Though the API endpoints are now being sanitized, and an SQL injection is no longer possible, the site as a whole is still insecure. There are still vulnerabilities(I have not included these in the writeup) that have not been fixed till date. I have been begging them to fix the issues for well over 2 years now (It goes way back to 2019. I did not even ask for something silly like money/bug-bounty or a hall of fame, btw, I openly told them all the flaws and they didn't have the decency to respond to me, or acknowledge my mails even once) and so, if anyone from Anima is reading this, fix your website and reply to mails!
