# Even and Odd number identifier.

number = int (input ("Please provide a number\n "))

# Check if the number is even or Odd 

typeCheck = number % 2

if typeCheck == 0:
    print ("We have an even number")

else:
    print ("You provided an odd number")
