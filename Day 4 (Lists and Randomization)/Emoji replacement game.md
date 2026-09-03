# The emoji game again
row1 = ["😵", "😴", "🙄"]
row2 = ["🤭", "🫣", "😳"]
row3 = ["😤", "🥳", "😒"]

# Put all the lists into one liist called map
map = [row1, row2, row3]

# display it on the console
print (f"{row1}\n{row2}\n{row3}")

# Ask the user the position they would like to change

position = input ("Where would you like to put the treasure?")

# split the positions into horizontal and vertical

hor =int (position[0] )
ver =int (position[1] )
# subtract the values by 1 because of offset 
vertical = ver - 1
horizontal = hor - 1

# Assign the position to the map

map1 = map[vertical]
# Change the item in the list by assigning the teasure "X"
map1[horizontal] = "X"

# display the new map

print (f"{row1}\n{row2}\n{row3}")
