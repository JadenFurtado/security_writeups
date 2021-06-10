### Anima Creatives management

The time I hacked a modelling agency. In all fairness, I tried my best to get the attention of the agencies involved here as well as people I knew who worked for them. 
Only when they did not respond to my mails and all other options that I tried failed, I decided to go ahead and exploit the vulnerabilities to get it to their attention so as to fix the flaws.

## Basic gist of the hack:
The website used a REST API to display images of the models. However, the inputs were not sanitized and this allowed me inject SQL into the website. I was able to extract the usernames and passwords from the database. The passwords were hased using the Md5 algorithm. I was able to reverse the hash using a rainbow table and log in as admin. 

# However, that is not all.
Though the API endpoints are now being sanitized, and an SQL injection is no longer possible, the site as a whole is still insecure. There are still vulnerabilities that have not been fixed till date. I however, am done trying to protect them! Some agencies never learn until it's too late...
