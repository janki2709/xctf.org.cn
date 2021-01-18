# xff_referer
Points: 2 Coin

## Category
Web

## Description
Teacher X told Xiaoning that xff and referer can be faked.

## Solution
By opening link, we get webpage stating   
ip address must be 123.123.123.123  
It's clear from the description that we either need to change X-Forwarded-For or Referer  
Value of X-Forwarded-For should be an IP Address and Value of Referer should be Website.  
So let's change the value of X-Forwarded-For:123.123.123.123  
Open the burpsuite and capture request.  
Add X-Forwarded-For:123.123.123.123 in the request.  
![X-Forwarded-For:123.123.123.123](https://github.com/janki2709/xctf.org.cn/blob/master/Exercise/Web/xff_referer/xff_referer.png)    
So, we got another webpage saying   
Must be from https://www.google.com   
Pretty clear we need to change Referer:https://www.google.com  
So, After changing the value   
X-Forwarded-For:123.123.123.123  
Referer:https://www.google.com  
![Referer:https://www.google.com](https://github.com/janki2709/xctf.org.cn/blob/master/Exercise/Web/xff_referer/xff_referer1.png)    
we Got the flag    
![X-Forwarded-For:123.123.123.123, Referer:https://www.google.com](https://github.com/janki2709/xctf.org.cn/blob/master/Exercise/Web/xff_referer/xff_referer2.png) 

## Flag
cyberpeace{8462de4134b9310ea1da679eadf04a6a}
