# cookie
Points: 1 Coin

## Category
Web

## Description
Teacher X told Xiao Ning that he put something in the cookie, Xiao Ning wondered: ‘Does this mean sandwich cookies? ’

## Solution
Open webpage, and according to Description we should think of cookies.  
So at first it can be something related to browser cookies but obviously it wasn't.  
We can't do anything with the webpage as it doesn't contain any input field or any button.  
So I just captured the request in the burpsuite as it was single hope for me.  
In the captured request we can find look-here=cookie.php  
So I simply opened cookie.php  
Then I got webpage stated that check the response. So again I captured that request send it to repeater and checked the response.  
I got the flag in the response.  
![notice that button is disabled](https://github.com/janki2709/xctf.org.cn/blob/master/Exercise/Web/disabled_button/disabled_button.png)  

## Flag
cyberpeace{604d2c1eacdf2ec2ef3ecae26464fdc1}
