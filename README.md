🎲 Dice Rolling Simulator (Python)

A simple Python project that simulates the rolling of a dice. This program uses the random module to generate a number between 1 and 6, mimicking the behavior of a physical dice. Great for beginners to learn about loops, functions, and user interaction in Python.

Features:

Random dice roll on each execution

ASCII representation of dice face

Option to roll again or exit


Code 

import random

def roll_dice():
    return random.randint(1, 6)

def main():
    print("Welcome to the Dice Rolling Simulator!")
    
    while True:
        input("Press Enter to roll the dice...")
        result = roll_dice()
        print(f"You rolled a {result}!")

        play_again = input("Do you want to roll again? (yes/no): ").strip().lower()
        if play_again != 'yes':
            print("Thank you for playing!")
            break

if __name__ == "__main__":
    main()
    
