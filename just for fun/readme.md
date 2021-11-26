# Just for fun:

## Introduction:

I have been feeling down in the dumps from the past few months, so, what better way to flip things than by going rouge as a hacker! 

Needless to say, this is just for fun and to get myself back in working order. Note to the reader: Do not abuse any of my findings

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

* If you do want to see how printers are exploited, check <a href="https://www.trendmicro.com/vinfo/in/threat-encyclopedia/vulnerability/164/buffer-overflow-in-print-spooler-vulnerability">this article</a> out

### Type 2 vulnerabilities: Incorrect configuration of web applications

Again, we will use google and search something along the lines of: " db_password filetype:env "

Clicking on one of the results that we get:

![image](https://user-images.githubusercontent.com/52862591/143563594-870717d1-421e-4a8c-8d53-646a0c5fd277.png)

I cropped out part of the password, but you can see that this application has been left with debug mode on as well as is disclosing the email-id and password of the sys-admin!🤦‍♂️

You can google the term I showed and see what all you can find. Again, no exploitation, just disclosure.

### Type 3: Password files exposed over the inernet

This is the most idiotic of all the vulnerabilities, where you have exposed passwords there for anyone to find if you know where to look for them

Just google the term  inurl:/wp-content/uploads/ ext:txt "username" | "user name" | "uname" | "user" | "userid" | "user id" AND "password" | "pass word" | "pwd" | "pw" 

![image](https://user-images.githubusercontent.com/52862591/143564935-8137f0a0-a3f1-43b4-bee7-c08ca53354cc.png)

I have cropped out the sensitive part. This is so easily avoidable, if all you do is keep the password file outside the website's root directory. Such a shame....

### Type 4: Online Cameras

While the idea of having a camera over the internet is for it to be easiy accessable, I am pretty certain, you don't want to grant a hacker access to security cameras!

Using google to search         intitle:"webcamxp" "Flash JPEG Stream"      and then clicking on the options, you can see that I now have access to the live stram of a camera

![image](https://user-images.githubusercontent.com/52862591/143568593-40f17143-59dd-464f-8285-7df644c78141.png)

I believe the above is of a european street. But we can see other stuff too like from security cameras on light poles as shown below

![image](https://user-images.githubusercontent.com/52862591/143569179-75df857e-d387-4b55-8ec3-7beb541f6836.png)

I don't think I need to explain why this is really bad!

The best way to stop unauthorized access is to use .htaccess to configure the endpoint


### Type 5: Plane boarding pass

Okay, while this is not exactly hacking and more of OSINT, I want to show why it is a terrible idea to post a picture of your boarding pass anywhere

Just google    "boarding pass" site:http://tripadvisor.com       and go to the image section of the search results

![image](https://user-images.githubusercontent.com/52862591/143566381-b3485317-e8ad-4dff-9b47-ac2c73adcb38.png)

You can try and decode the information present in the barcode using a simple barcode scanner app on your phone. I am pretty certain you do not want all that falling into the hands of a hacker or someone looking to play the fool with you.

As I won't be doing any exploitation, you can read more <a href="https://krebsonsecurity.com/2015/10/whats-in-a-boarding-pass-barcode-a-lot/">over here</a>



There still are a ton of things that I want to show, but that will be for another writeup.
