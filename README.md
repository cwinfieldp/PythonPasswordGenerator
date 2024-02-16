# PythonPasswordGenerator
Python Password Generator

#for loop

#Project - Password creator


import random


capital_let = "QWERTYUIOPASDFGHJKLZXCVBNM"
small_let = "qwertyuiopasdfghjklzxcvbnm"
numbers = "1234567890"
special_char = "?,.<>!%$]{£*|#@"
upper,lower,digits,odd = False,False,True,True

#Upper is linked with the 1st true, lower is linked with 2nd true, etc
#if you would like, it is also possible can also change some of the True statements to False to prevent some of the variables from   affecting how the passwords are generated


finalpass = ""


if upper:
    finalpass += capital_let
if lower:
    finalpass += small_let
if digits:
    finalpass += numbers
if odd:
    finalpass += special_char

#we are now linking finalpass and our variables

length = 15
howmuch = 10


for x in range(howmuch):
    password = "".join(random.sample(finalpass,length))
    
    print(password)
#we are now linking the quotation from line 14 and line 29
#random.sample will scramble the characters from letters numbers and special characters
#notice in the terminal there are 10 passwords from how much variable which are 15 characters long, which comes from the length variable
