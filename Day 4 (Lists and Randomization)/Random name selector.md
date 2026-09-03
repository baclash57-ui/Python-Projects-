# This is a program that selects a random name to pay the bills from the names provided without using the .choice function

# First import the random module
import random
# Ask the user to provide a name
names = input ("Hey there, put the names of the people you had a meal with today \n")

# Split the name variable to be seperated by ", " comma and a space bar 
names_string = names.split(", ")

# count the number of items in the list
number_of_strings = len(names_string)

# Index the list in a way that it would not exit the last item  
the_name = random.randint(0, number_of_strings - 1)

person_to_pay  = names_string[the_name]

# print out the name

print (f"The perosn to pay today is, {person_to_pay}" )
