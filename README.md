# Muggle-Game-PythonInstitute
This program is a game where there is a set number that the user must guess.  If the user guesses the number, 777, then the game is over.  If the user guesses any other number then the program asks them to guess again.  The user can type in 0 at anytime to end the game.

print(
"""
+================================+
| Welcome to my game, muggle!    |
| Enter an integer number        |
| and guess what number I've     |
| picked for you.                |
| So, what is the secret number? |
+================================+
""")

user_number = int(input("Choose any number between 1 and 1000! \nThe game will end if you hit the correct number!\nYou can always type in 0 to end the game!\nEnter number here: "))
while user_number != -1:
    if user_number == 777:
        print("Well done, muggle!  You are free now.")
        print("The game is over, goodbye!")
        user_number = -1
    elif user_number == 0:
        print("Giving up?  Try again next time then!")
        user_number = -1
    else:
        print("Ha ha! You're stuck in my loop!")
        user_number = int(input("Choose another number to leave!\nEnter new number here: "))
       
