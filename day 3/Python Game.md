# This is am interactive game that is affected by the user's choice of action

# Welcome the user
print (r"""

                                                    __________
             _,---.                          _..--'/          \
          ,-'      )                    _,-,'     /            \
         (          )               _,-'  /      /              \
          `-.__, -'             _,-/     /     _/ ,------------. \
     ,--._,---.             _,-'  /     /_,--'' | |    Hier    | |
   _(_,-'      )        _,-'/    /_, - '|       | |   koennte  | |
 ,'  (        )      ,'/   /_, -'|      ||_  -  | |    IRRE    | |
(     `--._,-'    _,' /_,-'|     ||_  - |       | |   Werbung  | |
 `--.__,-'     _,'/,-'|  - ||_ - |      ||_  -  | |   stehen!  | |
            _,'/,'|  - ___ |     ||_  - |       | `------------' |
        _ ,' |_' -|- _(   ) |_   |      ||_  -  |                |
       ( ): ((`) -| (. `-/ )   - ||_  - |       |                |
      ` | '(-.,') '( _\`/-') _ - |      | _   - |                |
        `   (_.) -(_._ \|,-_)    ||_  - |       |                |
 .        `. || ` | (_\||_)  _ - |      ||_  -  |                |
             `.    ` . ||  |   - ||_  - |       |                |
                `.     ||-.|  :  |  _   ||_   - |     __________ |
                   `.  ||    ` -.|   |  |   _   |    | _Doener_ |`'--.._
                      `.           ` - .|  | |  |    || ()._o  ||   __ |
\           `            `.   `           ` -' .|____|`'---.|>_||  |. ||
                            `.                         `' -- .._|__|__||
                      ,----.---------- .                            .-_.
   _                 |.`.,' `.           `.                         || |
    \                \ _|`. / `.            `.                      \|_o
     \                | \  `.   \.-----_-----.\     `
      \               `.|.`| `./ \\  c__)___/ \\             .
       \        `         `.   `. \\____\___)__\\
                            `. _ `.\`____________\
                              | \  |_|   ____   |_|
          _                   `.|\ |#|__[jrei]__|_|`.
           \                      `================'  `.



""")
print ("Hey there, welcome to lonard Island, Your goal is to esape the building")

Road = str (input ("Youre at an exit there are two doors, where do you want to go left or right?\n"))

# If the answer is left then they can proceed
if Road == "left":
# Ask the user if they want to wait for a boat or swim across the river

    patience = str ( input ("You come to a lake. Theres a key in the middle of the room surrounded by water. what will you do? Type 'Wait' to wait for a boat and 'Swim' to swim across?\n"))

# If the answer is 'wait' then they can proceed

    if patience == "wait":

        treasure = str( input ("You've arrived at the middle of the room unharmed,you've taken the key and 3 doors appear, One red, One Yellow and one blue. Which one do you want to choose?\n"))

    # If the ansqeer isn't yellow then the user can't proceed
     
        if treasure == "red":
            print ("Sorry gane over")

        elif treasure == "blue":
            print ("Sorry gane over")

        elif treasure == "yellow":
            print ("Hurray You win here's your theres a plane now you can go home")

        else:
            print ("Please enter any of the colours listed as an answer ")

    else:
         print ("Sorry game over...")

else :
    print ("Sorry, game over...")
