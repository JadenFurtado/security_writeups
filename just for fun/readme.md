# Just for fun:

## Introduction:

I don't usually do this kind of public disclosure, but to be honest, I have been struggling with myself over the past few months and I feel like I am losing control over my mind. So, what better way to flip things than by going rouge as a hacker! 

Needless to say, this is just for fun and to get myself back in working order. Note to myself and others: Do not abuse any of these findings

## Let's start hacking!

In this case, the entire internet is my target, using google to get whatever I want!

### Type 1 vulnerabilities: Insecure devices connected over the internet

How to find these? Just use google, because google is really powerful if used to its full potential

You can type something along the lines of: 	" intitle:HP LASERJET PRO MFP inurl:/SSI/index.htm  " and see a lot of interesting things pop up. 

This query uses google to list HP's laser jet printers

![image](https://user-images.githubusercontent.com/52862591/143561247-d1844def-a991-4ef2-a46f-133edec09058.png)

As you can see from the above screen shot there are a ton of options, where we can play around with the settings and other configurations of the printer
To someone who is not from a security background, this may not seem like much, after all, all that you could possibly do is print documents and maybe cause inconvenience to the owners. However, that is only partly true. You see, with a little knowledge on how printers work, you could take over the targets conputers just by using their printer! 

How? 

Because of something called spooling. It is essentially a buffer that is used by devices such as printers to speed up the printing process. See the image below

![image](https://user-images.githubusercontent.com/52862591/143562556-b2145135-fa50-4b9a-bba4-b42aea1c34da.png)

Spooling is notorious for buffer overflow vulnerabilities. I won't exploit this as I said before, only me disclosing vulnerabilities.

### Type 2 vulnerabilities: Incorrect configuration of web applications

Again, we will use google and search something along the lines of: " db_password filetype:env "

Clicking on one of the results that we get:

![image](https://user-images.githubusercontent.com/52862591/143563594-870717d1-421e-4a8c-8d53-646a0c5fd277.png)

I cropped out part of the password, but you can see that this application has been left with debug mode on as well as is disclosing the email-id and password of the sys-admin!🤦‍♂️

You can google the term I showed and see what all you can find. Again, no exploitation, just disclosure

### Type 3: Password files exposed over the inernet

This is the most idiotic of all the vulnerabilities, where you have exposed passwords there for anyone to find if you know where to look for them

Just google the term  inurl:/wp-content/uploads/ ext:txt "username" | "user name" | "uname" | "user" | "userid" | "user id" AND "password" | "pass word" | "pwd" | "pw" 

![image](https://user-images.githubusercontent.com/52862591/143564935-8137f0a0-a3f1-43b4-bee7-c08ca53354cc.png)

This is so easily avoidable, if all you do is keep the password file outside the website's root directory. Such a shame....


