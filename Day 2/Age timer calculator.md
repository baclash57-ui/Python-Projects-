# This program  calculates the amount of Days, weeks and months a user has left till their 90

#Greeet the user
print ("Hey there, you want to know how much time you have left? \nThat's cool I'll help you out")

# Ask the User for their Age 
UserAge = int(input ("Wow old are you? \n")) 

#Subgtract the age from 90
Ageleft = 90 - UserAge

# Calculate their age left in days weeks and months with the number of days as 365

DaysLeft = Ageleft * 365 
MonthsLeft = Ageleft * 12
WeeksLeft = Ageleft * 52

# display the time left in days, weeks and months
print (f"Okay you have  {DaysLeft} days , {MonthsLeft} months and {WeeksLeft} Weeks left \nUse your life welll!!")
