# This program cvhecks if a number is even or odd 
print ("Let's check if a number is even or odd shall we...")
Number= int (input("Please enter a number.\n")) 

# Check if the numner is even or odd 
checkNum = Number % 2 

if checkNum == 0:
    print ("It's an Even number")
else:
    print("It's an Odd number")
