# This is a program that calculates the tip to be paid for a meal

# greet the User
print ("Hey there, Welcome to the tip calculator. \n I'll help you and your friends split the bill no matter the tip")

# Ask the price of the bill

Bill = float(input ("How much is the bill? \n"))

# Ask how many people are splitting the bill
people =  int(input("how amny people are splitting the bill? \n"))

# Ask for the interest rate 
rate = float (input("At what rate? \n"))

# Calculate the price for each person

Price = round ((Bill / people) * (1 + (rate / 100)) ,2) 

# Display the price of the  bill

print  (f"Each of you will pay {Price}" )
