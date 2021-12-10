# Let's talk common sense in cybersecurity and software development,
## because common sense is not that common!

* These are taken from my past experiences

### Storing passwords in plain text:
Please don't store passwords in plain texts 🙏. 

![image](https://www.savethestudent.org/uploads/easy-password.jpg)

### Storing password hints and plain text password next to the hash:
The skill and genius required for this is out of this world and yet I have come across this in real life!

![image](https://user-images.githubusercontent.com/52862591/145393094-a71f42d5-ed62-4a14-83a2-1f696249ca6a.png)

Why even bother to hash the passwords in the 1st place if you are storing the plain text password?

### Returning sensitive information to all users:
Just fetching information and not displaying it does not make an application secure! It just hides the information from the regular user, that's all.
Below is a real example that discloses the IP, Pan card number, Address, mobile number, password, email-id and a ton of other data

![image](https://user-images.githubusercontent.com/52862591/145393931-b8f122e4-58e5-44b6-b870-55455b4e0e8f.png)

### Not sanitizing user inputs:

General rule of thumb in coding, do not trust your users! You never know what they might cook up

![image](https://user-images.githubusercontent.com/52862591/145395094-78f6b133-cdb2-401d-abc6-2d34680401df.png)

### Depending on a WAF to shield against an intrusion

While using a WAF is good and all, depending on it alone is not good enough. Why? see the below gif

![Firewall Vs Hacker](https://i.makeagif.com/media/3-19-2018/Dm3nrC.gif)
