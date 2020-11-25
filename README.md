# Rock-Paper-Scissor-game
from random import randint
t = ["Rock", "Paper", "Scissor"]
computer = t[randint(0,2)]
player = False
while player == False:
    player = input("Choose one from the following Rock, Paper, Scissor\n")
    if player == computer:
        print("Tie")
    elif player == "Rock":
        if computer == "Paper":
            print("You loose!", computer, "covers", player)
        else:
            print("You win!", player, "smashes", computer)
    elif player == "Paper":
        if computer == "Scissor":
            print("You loose!", computer, "cut", player)
        else:
            print("You win!", player, "covers", computer)
    elif player == "Scissor":
        if computer == ("Rock"):
            print("You loose!", computer, "smashes", player)
        else:
            print("You win!", player, "cut", computer)
    else:
        print("Enter correct spelling!!!")
    player == False
    computer = t[randint(0,2)]
