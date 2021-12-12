# All you need to know about Passwords

<i>Note: All information is purely for knowledge and for developers only. 
  I am not responsible for any misuse of the information that I am providing in either this or any other writeup. Please do not break the law!
  In India, Section 66 of the IT Act deals with the offence of computer hacking. 
  In simple words, hacking is accessing of a computer system without the express or implied permission of the owner of that computer system. 
  The punishment for hacking is imprisonment upto 3 years or fine which may extend to 2 lakh Rupees or both.</i>

### Passwords, the nightmare of every CISO and the friend of every hacker/pen-tester! Here is a crash course on all you need to know about passwords

## Finding breached accounts:
I am starting off with this because I think it is important to understand why 2FA is necessary for all your accounts. On googling something along the lines of:

![image](https://user-images.githubusercontent.com/52862591/145716956-587369c2-a431-4215-8421-4402de70f68b.png)

and then check some of the results, we find that there are millions of accounts that have already been breached and their passwords posted on sites such as pastebin. 

![image](https://user-images.githubusercontent.com/52862591/145717091-c1f09e2c-a019-45a9-b4cd-5fe1815087c7.png)

This is what makes 2FA so important in 21st century. Breaches happen every day and there is no knowing when it may be your turn.

## How to store passwords?
Do not store passwords in plain text or encrypt passwords or just hash passwords, rather, hash passwords along with a salt and pepper to prevent frequency 
