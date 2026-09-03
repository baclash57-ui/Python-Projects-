# Rock paper scissors 

# import the raandom module
import random
# This program randomly gives aither rock, paper or scissors  when the user selects one

# Greet the user 
print ("hey there, welcome to the RPS game.")

rock = """
    _______
---'   (____)
      (_____)
      (_____)
      (____)
---.__(___)
"""

paper = """
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
"""

scissors = """
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
"""


# Ask them to pick a number with respect to the three options
choice =int  (input ("What do you choose? type 0 for rock, 1 for paper and 2 for scissors\n"))


# Put the three items in a list
game = [rock, paper, scissors]
# we can use the "random.choice()" function but that wouldn't strenghten our understanding of indexing
    # count the number of items in the variable game  

    # randomize it
ans = random.randint(0, 2)
# set the condition for the choice the user makes

if choice == 0:
    print (rock)

    response = game[ans]
    print(f"Computer choose {response}")

    #calculate the answer

    if response == paper:
        print ("Aw sorry you lose")
    elif response == scissors:
        print ("Yay you win")
    elif response == rock:
        print ("It's a draw, Lets try that again shall we")
        
elif choice == 1:
    print (paper)

    response = game[ans]
    print(f"Computer choose: {response}")
     #calculate the answer
    if response == scissors:
        print ("Aw sorry you lose")
    elif response == rock:
        print ("Yay you win")
    elif response == paper:
        print ("It's a draw, Lets try that again shall we")

elif choice == 2:
    print (scissors)

    response = game[ans]
    print(f"Computer choose: {response}")
    #calculate the answer
    if response == rock:
        print ("Aw sorry you lose")
    elif response == paper:
        print ("Yay you win")
    elif response == scissors:
         print ("it's a draw, Lets try that again shall we")

else:
    print ("You typed an invalid number, you lose!") 
