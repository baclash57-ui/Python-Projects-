students_height = input ("Input a list of student heights \n").split()

for n in range(0, len(students_height)):
    students_height[n] = int (students_height[n])

print(students_height)

total_height = 0
for height in students_height :
    total_height += height

print (f"The total height is {total_height}")

student = 0
for sutdents in students_height:
    student += 1

print (f"the total numner of dtudents is  {student}")

avg =round ( total_height / student)

print (f"the average is {avg}")
