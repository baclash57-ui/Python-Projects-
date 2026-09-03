# this program calculates the chances that your crush is actually your true love and shows it as a whole percentage

# Greet the User 
print ("hey there trying to know if your crush is your true love? Don't worry i've got you covered...")

# Ask them for their first and last names and the first and last namse of their Crush
Name = input("What are  your first and last names?\n")
Crush = input ("What are the first and last names of your crush?\n")

 # Combine both names into one 
Both_names = Name + Crush

#make it lower case
both = Both_names.lower()

# Display the name in the console
print (f"Hey there {Name}")

# Compare the name with the number of times the letters T-R-U-E and L-O-V-E 
Count_true = both.count("t") + both.count("r") + both.count("u") + both.count("e")
Count_love = both.count("l") + both.count("o") + both.count ("v") + both.count ('e')


# convert the variables to strings 
Total_true = str(Count_true) +  str (Count_love)


# save them as Total
Total = int (Total_true)

# Add condition to interprete the score 
if (Total < 10) or (Total > 90):
    print (f"Wow your love score is {Total}% , You go together like coke and menthos")

elif  range (Total, 40,50 ):
    print (f"Oh my your love score is {Total}%, You guys are perfect") 
else:
    print (f"Your love score is {Total}%")    
