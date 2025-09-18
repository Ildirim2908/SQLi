# Lab Description says

![SQLi PoC](images/17.png)

# Let's check the presence of sql injection by ' sign 

![SQLi PoC](images/18.png)

## as we see we got an error which potentially indicates that application is vulnerable to sql injection

# Let's see how many columns are queryed in original query on backend with order by technique

![SQLi PoC](images/19.png)

## two columns are queryed

# Let's see what database is used

![SQLi PoC](images/20.png)

## Oracle database is used

# It is time to enumerate table names to see where username and passwords could be stored

![SQLi PoC](images/22.png)

this is the payload that is used to retrieve table names

![SQLi PoC](images/21.png)

## this table seems to be the one

# When we retrieve columns we get this result

![SQLi PoC](images/23.png)

# And Finally let's see what is inside these columns

![SQLi PoC](images/24.png)


## and we see passwords of administrator and some other users

![SQLi PoC](images/25.png)
