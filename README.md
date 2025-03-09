#import
import random 

#numbers
lowest_numbers = 1
highest_numbers = 25
correctnumber = random.randint(lowest_numbers, highest_numbers)

#askingname
player1 = input("Enter your name player1")
player2 = input("Enter your name player2")

player1 = "player1"
player2 = "player2"

#to keep user guessing
guesses = 0
#running
is_it_running = True

#player1

#Welcome
print("This is a Python two player guessing game guessing game")
print(f"Select a number from {lowest_numbers} and {highest_numbers} :  ")

#checking if correct or not
while is_it_running:
      guess = input("Enter a guess: ")

#typecasting/adding 1 to guesses
      if guess.isdigit() :
         guess = int(guess)
         guesses += 1

#if types out more or lower
         if guess < lowest_numbers or  guess >  highest_numbers :
            print("That number is invalid")
            print(f"Please Select a number from {lowest_numbers} and {highest_numbers} :  ")

#if to low
         elif guess < correctnumber:
             print("Too LOW!")

#if too high
         elif guess > correctnumber:
             print("Too HIGH!")
#if correct             
         else :
             print(f" CORRECT IT IS! {correctnumber}") 
             print(f"It took you {guesses} guesses")  
             is_it_running = False
#if invalid             
      else:
         print("Invalid Statement")
         print(f"Please Select a number from {lowest_numbers} and {highest_numbers} :  ")

#player2
print("It is the secong player turn")
print(f"Select a number from {lowest_numbers} and {highest_numbers} :  ")

#checking if correct or not
while is_it_running:
      guess = input("Enter a guess: ")

#typecasting/adding 1 to guesses
      if guess.isdigit() :
         guess = int(guess)
         guesses += 1

#if types out more or lower
         if guess < lowest_numbers or  guess >  highest_numbers :
            print("That number is invalid")
            print(f"Please Select a number from {lowest_numbers} and {highest_numbers} :  ")

#if to low
         elif guess < correctnumber:
             print("Too LOW!")

#if too high
         elif guess > correctnumber:
             print("Too HIGH!")
#if correct             
         else :
             print(f" CORRECT IT IS! {correctnumber}") 
             print(f"It took you {guesses} guesses")  
             is_it_running = False
#if invalid             
      else:
         print("Invalid Statement")
         print(f"Please Select a number from {lowest_numbers} and {highest_numbers} :  ")
