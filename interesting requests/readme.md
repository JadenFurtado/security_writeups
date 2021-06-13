# Interesting requests

## Inroduction:

Was looking for an internship on Internshala when I came across RISEE’s website. I decided to check their site out and it became apparent that they have a few flaws. On investigating further, I saw that they have a leaking API. I was able to successfully log in as another user thanks to exposed user id’s and user refresh tokens. 

## Full writeup : https://github.com/JadenFurtado/security_writeups/blob/main/intersting%20requests/Interesting%20requests.pdf

### The admin's account:

<img src="https://github.com/JadenFurtado/security_writeups/blob/main/interesting%20requests/risee_profile.png" />

## timeline:

### 7th June 2021, 17:00 : Looking for an internship on internshala, I come across an internship from RISEE an decide to visit their site
### 7th June 2021, 18:30 : I discover that they have a leaking API, but can't think of how to exploit it. Got an exam the next day, so have to study and put it at the back of my mind.
### 8th June 2021, 21:30 : I revisit RISEE. I decide not to inform them until I have a working POC. I intercepted their server requests using Burp and modify them
### 8th June 2021, 22:00 : I have logged in as a user of their site
### 8th June 2021, 22:10 : I have logged in as admin
### 8th June 2021, 00:23 : I write a mail to RISEE informing them of my findings.
