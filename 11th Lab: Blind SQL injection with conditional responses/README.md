# Lab Description says
![SQLi PoC](images/46.png)
## as it states sql injection is in tracking cookie and when we get error from database "Welcome back!" message isn't returned and we will use blind sql injection method to retrieve data from database
# When just sending normal request we get Welcome back! message
![SQLi PoC](images/48.png)
## however if we send slightly edited Tracking cookie value we dont receive Welcome back! anymore
![SQLi PoC](images/49.png)
# POC of blind sqli being present by adding to payload (and '1'='1/ and '1'='2)
![SQLi PoC](images/51.png)
![SQLi PoC](images/52.png)
# We will retrieve data by comparing each character of desired column value with alphanumeric characters that we choose
![SQLi PoC](images/53.png)
## in this case we are comparing if first letter of administrator's password is less than 'm' and if it is less we are returned "Welcome back!" message, if first letter's ascii integer value was more than of m's we wouldn't have been returned "Welcome back!" message
# By comparing more and more we equal first letter of administrator's password to 'h' and we are returned "Welcome back!" which means that first letter of password is indeed h
![SQLi PoC](images/54.png)
## but to make things faster and automize everything I will use Burp's intruder section to do it
![SQLi PoC](images/59.png)
### this is how payload will look 
### every time I will get successful result I will increment "SUBSTRING((SELECT password FROM users WHERE username = 'administrator'), #1#, 1)" in this payload first one, the one that i added # sign

