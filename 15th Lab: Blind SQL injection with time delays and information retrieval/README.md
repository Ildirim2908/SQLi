# Lab Description says
![SQLi PoC](images/81.png)
## we will use time based SQL injection to retrieve information from database
# Checkgin for time delay by injecting pg_sleep()
![SQLi PoC](images/1.gif)
# Retrieving password of administrator user
![SQLi PoC](images/2.gif)
## with this method by trial and errors in the end we will get what is the first character of administrator user's password however to make things faster i have sent this request to intruder
![SQLi PoC](images/82.png)
## and from the response we see that successful character took 2 seconds to be responded and by this we take notes of every character of password
![SQLi PoC](images/83.png)
# Solved
![SQLi PoC](images/84.png)
