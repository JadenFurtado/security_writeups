# Anima Creatives management

The time I hacked a modelling agency. In all fairness, I tried my best to get the attention of the agencies involved here as well as people I knew who worked for them. 
Only when they did not respond to my mails and all other options that I tried failed, I decided to go ahead and exploit the vulnerabilities to get it to their attention so as to fix the flaws.

## Basic gist of the hack:
The website used a REST API to display images of the models. However, the inputs were not sanitized and this allowed me inject SQL into the website. I was able to extract the usernames and passwords from the database. The passwords were hased using the Md5 algorithm. I was able to reverse the hash using a rainbow table and log in as admin. 

### However, this is not all. I have not included this section in the writeup.

The director of anima asked me not to include their name in the writeup. However, I think it's only fair that I do it, for the following reason.

Though the API endpoints are now being sanitized, and an SQL injection is no longer possible, the site as a whole is still insecure. There are still vulnerabilities(I have not included these in the writeup) that have not been fixed till date. I have been begging them to fix the issues for well over 2 years now (It goes way back to 2019. I did not even ask for something silly like money/bug-bounty or a hall of fame, btw, I openly told you'll the flaws) and I am done trying to protect them and their employees! I guess some agencies never learn until it's too late. If they get hacked(wouldn’t surprise me), too bad, but then again, that is not my problem and they can't blame me. I had given you guys a head start from 2019!
