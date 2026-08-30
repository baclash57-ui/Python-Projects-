# provide a  two digit number and then add the digits together
two_digit_number = input("Provide a two digit number\n ")

# check fot the data type
print (type(two_digit_number))

# Collect the first and second values

no1 = two_digit_number[0]

no2 = two_digit_number[1]

# Display the values to the 
print(no1)
print(no2)

# add the digits of the number

Digit = int(no1) + int(no2)

# COnvert the variable into a string
newDigit = str (Digit)

# Display it 
print("your new number is..." + newDigit)
