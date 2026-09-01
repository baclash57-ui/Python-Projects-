# Program that calculates if a year is a leap year

print ("Hey there trying to find out the next leap year? \nDon't worry I gotcha")

# Ask the user to provide a year
Year = int (input ("Please enter a year \n"))

# Check if this is a leap year 
if Year % 4 == 0:
    
    if Year % 100 == 0:
        print ("This is not a leap year")

        if Year % 400 == 0:
            print ("This is a leap year")
else:
    print("This is not a leap Year")
