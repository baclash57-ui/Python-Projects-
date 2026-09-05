# This code runs when the Use inputs a range of scores seperated by a space.

student_Scores = input ("Input a list of student scores\n").split()

for n in range (0, len(student_Scores)):
    student_Scores[n] = int (student_Scores[n])
    
print (student_Scores)


highest_score = 0
for score in student_Scores:
    if highest_score < score:
        highest_score = score

print(f" the highest score is {highest_score}")

# Declare a variable with the value 0 for comparison 
Lowest_var = student_Scores[0]

# Go through the loop and compare the values to find the lowest
for score in student_Scores:

    # compare the value of the items in the list with the variable and print out the lowest variable
    if score <  Lowest_var:
        Lowest_var = score

print (f" The Lowest score in the class is {Lowest_var}")

