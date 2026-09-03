# This is a virtual coin toss program, that gives heads or tails if the random number generated is even or odd

# First import the random module
import random

random_number = random.randint(1,100)
print (random_number)

if random_number % 2 == 0:
     print ("Heads")
else:
    print ("Tails")

# Random toss another style

# toss = ["heads", "tails"]

# print (random.choice(toss))
