# This code calculates the BMI of an induividual based on the height and weight they provide

#Greet the person
print ("Hey there welcome to the BMI calculator.\m We just need a few things to get statred")

# Ask the person for their height and weight

height = float (input ("Whats your height in Meters? \n"))

weight = int (input ("Whats your weight in lps? \n"))

# Calculate the BMI of the person

BMI =  round (weight / (height)**2)

# Print the BMI 
print (f"Your BMI is {BMI}")
