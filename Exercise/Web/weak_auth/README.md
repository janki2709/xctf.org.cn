# weak_auth
Points: 1 Coin

## Category
Web

## Description
Xiao Ning wrote a login verification page and set a password at hand.

## Solution
First I entered anything and I got prompt message Saying please login as admin.  
So it was confirm that username is admin. Now I need to think about password.   
At first I thought may be SQL Injection can work. So I tried different SQL Injection payloads but this thing didn't worked.  
Then I thought to bypass login by using Burpsuite but this also didn't worked.  
Then I opened page source after entering anything in the password field.  
I got hint in the source code <!--maybe you need a dictionary-->  
Now I got that it's a dictionary attack  
I immediately found this wordlist  
https://github.com/fuzzdb-project/fuzzdb/blob/master/wordlists-user-passwd/passwds/john.txt   
I tried this wordlist with burpsuite.  
Capture request in the burpsuite, then send it to intruder.  
Go to position->clear. Then click on passsword->add.  
Go to payloads and Select the payload and start attack.  
After finishing attack, check response(click on response)  
Check response of every single payload.  
I got flag at 5th payload only.   
Password is 123456  

## Flag
cyberpeace{26c25f5a7d279bac6c991d896bc7429d}
