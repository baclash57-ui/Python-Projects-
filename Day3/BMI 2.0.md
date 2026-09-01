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


# assert their level of bidy mass

if BMI <= 18.5:
    print ("Looks like you're under weight, you need to start eating some fruits and vegetables")

elif BMI < 26:
    print("Your weight is normal, you're a healty person")

elif BMI < 31 :
    print ("You're overweight")

elif BMI <= 35:
    print ("You're obesed please start working out")

elif BMI > 35:
    print ("You're crytically obessed, we need to watch your diet.")
   

 
