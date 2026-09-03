# program on conditional statements. This program is to allow people over 120 cm to ride a roller coaster

# Greet the user
print ("Welcome to the Scrudd Roller coaster, you ready to have a blast?")

# Ask the user for their height
height = int (input ("Before we start, how tall are you in cm? \n"))

# Check if the height is greater tha 120 cm if it is then you allow then to enter.

if height >=  120:
    print ("Welcome aboar, Enjoy your ride!!")

    age = int (input ("How old are you?\n"))

    ticket = 0

    if age < 12:
        ticket += 5
        print ( f" Tickets for children are ${ticket}.")

        # Ask the user if they would like a photo

        photo = bool (input ("Would you like to take a photo? \n Y or N \n"))

        
        # Calculate the new bill
        newbill = ticket + 3

        if photo == "Y" :
            print (f"Your tcket is {newbill}")
        else:
            print (f"Your ticket is {ticket}")

    elif age < 18:
        ticket += 7
        print (f"Tickets for Teenagers are ${ticket}.")

         # Ask the user if they would like a photo
        
        photo = bool (input ("Would you like to take a photo? \n Y or N \n"))
        
                
        # Calculate the new bill
        newbill = ticket + 3
        
        if photo == "Y" :
            print (f"Your tcket is {newbill}")
        else:
            print (f"Your ticket is {ticket}")
            

    elif age >= 18:
        if age >= 45 and age <= 55:
            print ("Your Tickets are free")

        else:
            ticket += 12
            print (f"Adult tickets are ${ticket}.")

         # Ask the user if they would like a photo
        
        photo = bool (input ("Would you like to take a photo? \n Y or N \n"))
                
        # Calculate the new bill
        newbill = ticket + 3
        
        if photo == "Y" :
            if age >= 45 and age <= 55:
                print ("Your ticcket is free")
            else:    
                print (f"Your tcket is {newbill}")
        else:
            if age >= 45 and age <= 55:
                print ("Your ticcket is free")
            else:
                print (f"Your ticket is {ticket}")

 # If height is less than 120 cm, then don't allow them to enter
else:
    print ("Sorry wait until you're taller....")
