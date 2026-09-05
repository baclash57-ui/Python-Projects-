# Passowrd generator 
import random

letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z' 
           'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']

numbers =['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+' ]

print ("Welcome to the pypassword generator!")
nr_letters = int (input(f"How many letters would you like in your password?\n"))
nr_symbols = int (input(f"how many symbols would you like?\n"))
nr_numbers = int (input (f"How many numbers would you like?\n"))

#Catch the number of items in the lists
no_of_letters = len(letters)
no_of_numbers = len(numbers)
no_of_symbols = len(symbols)


password = ""

# Easy way

for letr in range (0, nr_letters + 1):
    password += random.choice(letters)
    # print (password)

for symbs in range (0, nr_symbols):
    password += random.choice (symbols)
    # print (password)

for numbs in range (1, nr_numbers + 1):
    password += random.choice (numbers)
    # print (password)

# print (f"Your password is {password}")

# The hard way 

# Make an empty list 
password_list = []

# Append the random number of items in the other lists to it
for letr in range (0, nr_letters + 1):
    password_list.append(random.choice(letters))
    # print (password)

for symbs in range (0, nr_symbols):
    password_list.append (random.choice (symbols))
    # print (password)

for numbs in range (1, nr_numbers + 1):
    password_list.append (random.choice (numbers))
    # print (password)

# Display the items in the list

# print (f"Your password is {password_list}")

# SHuffle the items in the list 

random.shuffle(password_list)
# print (f"Your password is {password_list}")

# Now print it as a string
a = ""
for items in password_list:
    a += items
print(f" Your password is {a}")

