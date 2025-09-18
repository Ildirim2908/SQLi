# Lab Description says
![SQLi PoC](images/40.png)

# Enumerating number of columns in original query 
![SQLi PoC](images/39.png)
## (2 columns)

# Let's see in which column we can input string
![SQLi PoC](images/41.png)
## this one returned an error so we should inject string type in second column
![SQLi PoC](images/42.png)
# Concatenation of two values into one column 
![SQLi PoC](images/43.png)
## here i have shown that if we concat with this "||" sign only we get everything next to each other however we can seperate values by simple techinque that is shown in next screenshot
![SQLi PoC](images/44.png)
# Lab Solved
![SQLi PoC](images/45.png)
