# This is a program that calculates the price of pizza based on what the user chooses

# Greet the user 
print("hey there, welcome to python Pizza Derliveries!")

size = input("What size of Pizza do you want? S, M, or L? \n")

add_pepperoni = input ("Do you want some pepperoni? Y or N? \n")

extra_Cheese = input ("Do you want extra cheese? Y or N \n")

bill = 0

# Add conditional checks for the project
if size == "S":
    bill += 15

if size == "M":
    bill += 20

if size == "L":
    bill += 25

# Check for the price if pepperoni is added 

if add_pepperoni == "Y":
    if size == "S":
        bill += 2
        print (f"That would be ${bill} please.")
    else :
        bill += 3
        print (f"That would be ${bill} ")
        
# Check for the price if cheese is added 

if extra_Cheese == "Y":
    bill += 1
    print (f"So every thing will be ${bill}. Enjoy your pizza!")
    
    
