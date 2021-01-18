# get_post
Points: 2 Coin

## Category
Web

## Description
Teacher X told Xiao Ning that HTTP usually uses two request methods. Do you know which two are?

## Solution
We know that HTTP usually uses GET and POST request methods.
By opening challenge URL, we get webpage saying 
Please use GET to submit a variable named a and value 1
So submit URL by appending ?a=1
We get another webpage saying
Please use GET to submit a variable named a and value 1
Please use POST to submit a variable named b with a value of 2.
![check response](https://github.com/janki2709/xctf.org.cn/blob/master/Exercise/Web/weak_auth/weak_auth1.png)
I tried to submit post value b=2 with burpsuite but it didn't worked, I don't know why
So, I go for Hackbar(Popular firefox/chrome extension) 
Submitted post request with b=2 and get request ?a=1
Got the flag

## Flag
cyberpeace{97559ea355b01f074e65598ebdcfe3cf}
