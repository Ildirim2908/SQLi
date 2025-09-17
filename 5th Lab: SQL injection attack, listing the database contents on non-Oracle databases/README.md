# Lab Description says

![SQLi PoC](images/1.png.png)

## We will need to inject a payload to get the password of the users on the system so let's start

# Normal output of web application 

![SQLi PoC](images/2.png.png)

# Let's try injecting ' sign to detect if application is vulnerable to sql injection

![SQLi PoC](images/3.png.png)

as we see we got an error indicating that indeed application may be vulnerable

# Detecting number of columns in original query written on backend of application (2)

![SQLi PoC](images/4.png.png)


# Let's try retrieving database version to inject payloads comfortably in future

![SQLi PoC](images/5.png.png)


# injecting payload to get table_names to see where could be username and password stored


![SQLi PoC](images/6.png.png)

![SQLi PoC](images/7.png.png)
