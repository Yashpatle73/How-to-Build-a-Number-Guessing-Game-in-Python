# How-to-Build-a-Number-Guessing-Game-in-Python
#In this project, you will create a simple number guessing game that allows the user to guess a random number between 1 and 100. The program will give hints to the user after each guess, indicating whether their guess was too high or too low, until the user guesses the correct number
import random

secret_number = random.randint(1, 100)

while True:
    guess = int(input("Guess the number between 1 and 100: "))
    
    if guess == secret_number:
        print("Congratulations! You guessed the number!")
        break
    elif guess < secret_number:
        print("Too low! Try again.")
    else:
        print("Too high! Try again.")
