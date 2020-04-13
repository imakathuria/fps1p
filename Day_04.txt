"""
1. Business Development Team

2. Business Analyst - gather the requirement
(features list)
Project Specifications

3. Technical Team (Development Team)
Architect - design the flow (design document)

4. Testing team, test cases, JIRA, bug(issues)

5. Release/Deployment/Production

6. Incrementatl Development

(Software Development Life Cycle - SDLC)
Agile Methodology - SCRUM, Sprint


Bugs
1. Draw case is not handeled
2. Issue with input (case sensitivity)
user_input.lower()
3. Check for invalid input, if invalid, show the message to user for correct input

New requirement from the client
1. Score Board


GUI - Graphical User Internface
1. Tkinter
2. WxPython
3. Qt5


Git
Bitbucket
SVN Tortoise
Perforce
"""

#difference between binary file and text file


"""
Make a game of rock, paper scissors against the computer. 
Problem
    Tell the user about the Game Instruction
    Tell user to enter either rock,paper or scissors
    Get the response from the user 
    
    Generate a random choice from (rock, paper, scissors)
    Compare user selection and computer selection
    Display who wins.
Extension
    Make sure the user enters a valid entry.
    Add a loop structure to play several times and keep a running score
    
Hint
  Rock  vs paper   -> paper wins
  Rock  vs scissor -> Rock wins
  paper vs scissor -> scissor wins

"""
# Algorithm  
"""
Print the Game Instruction to the User/Player
    
Infinite Loop 
    Tell User to enter either Rock, Paper, Scissor
    Get the response from the User
    Print the response from the User
    
    Computer chooses randomly between Rock, Paper and Scissor
    Print computers choice
    Print User Choice and Computer Choice
    
    
    Decide the condition of wining according to the Game Instructions
    
    
    Compare the result with user and computer 
    Printing either user or computer wins 
    
    
    Get the response from User to Play Again
    Check the response from User and continue the loop
    Othewise break the loop to close the game


Print a Thanks Message to the user
"""

# Step 1
###############################################################################

# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs Paper   -> Paper wins \n"
                                +"\tRock  vs Scissor -> Rock wins \n"
                                +"\tPaper vs Scissor -> Scissor wins \n") 




# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 


# Step 2
###############################################################################
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:


    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Othewise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 


# Step 3
###############################################################################

# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    
    


    
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Othewise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 


# Step 4
###############################################################################
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    
    
    
    
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Othewise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 


# Step 5
###############################################################################

# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
          
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    else: 
        result = "scissor"
    
    
    
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Othewise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 


# Step 6 
###############################################################################
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
          
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins
    
    if (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
    
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 

###############################################################################
"""
Final Version 1
"""
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
          
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins  
    if (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
      
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 
###############################################################################




###############################################################################
"""
Final Version 2
"""
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    elif(user_choice == "rock" and comp_choice == "rock"): #additonal
        result = "rock"
    elif(user_choice == "paper" and comp_choice == "paper"): #additional
        result = "paper"
    elif(user_choice == "scissor" and comp_choice == "scissor"): #additional
       result = "scissor"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins  
    if (result == user_choice and result == comp_choice): #additional
        print("<== Draw ==>") 
    elif (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
      
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 
###############################################################################



"""
Final Version 3
"""
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
    user_choice = user_choice.lower()
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    elif(user_choice == "rock" and comp_choice == "rock"): #additonal
        result = "rock"
    elif(user_choice == "paper" and comp_choice == "paper"): #additional
        result = "paper"
    elif(user_choice == "scissor" and comp_choice == "scissor"): #additional
       result = "scissor"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins  
    if (result == user_choice and result == comp_choice): #additional
        print("<== Draw ==>") 
    elif (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
      
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 
###############################################################################








"""
Final Version 4
"""
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
      
    # Get the response from the User 
    user_choice = input("User turn: > ") 
    user_choice = user_choice.lower()
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins  
    if (user_choice == comp_choice): #additional
        print("<== Draw ==>") 
    elif (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
      
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 
###############################################################################


#Now guys, you are given a assignment, do not allow user to enter anything except
#rock, paper, scissors



"""
Final Version 5
"""
# Print the Game Instruction to the User/Player 
print("Winning Rules of the Rock Paper Scissor Game as follows: \n"
                                +"\tRock  vs paper   -> paper wins \n"
                                +"\tRock  vs scissor -> Rock wins \n"
                                +"\tpaper vs scissor -> scissor wins \n") 

while True:

    # Tell User to enter either Rock, Paper, Scissor    
    print("Enter choice \n 1. rock \n 2. paper \n 3. scissor \n") 
    
    while True:
        # Get the response from the User 
        user_choice = input("User turn: > ") 
        user_choice = user_choice.lower()
        
        if user_choice not in ['rock','paper','scissor']:
            print ("Wrong input, please input again: ")
        else:
            break
 
    # Print the response from the User 
    print("User has choosen : " + user_choice + "\n") 
    

    
    # Computer chooses randomly between Rock, Paper and Scissor
    import random
    comp_choice = random.choice(['rock','paper','scissor']) 

    # Print computers choice
    print("Computer choice is: " + comp_choice + "\n") 
  
    # Print User Choice and Computer Choice
    print("\t" + user_choice + "\n V/s \n" + "\t"+ comp_choice) 
    

    # Decide the condition of wining according to the Game Instructions
    result = None
    
    if((user_choice == "rock" and comp_choice == "paper") or
      (user_choice == "paper" and comp_choice == "rock" )): 
        result = "paper"
    elif((user_choice == "rock" and comp_choice == "scissor") or
        (user_choice == "scissor" and comp_choice == "rock")): 
        result = "rock"
    else: 
        result = "scissor"
    

    # Compare the result with user and computer 
    # Printing either user or computer wins  
    if (user_choice == comp_choice): #additional
        print("<== Draw ==>") 
    elif (result == user_choice): 
        print("<== User wins ==>") 
    else: 
        print("<== Computer wins ==>") 
    
      
    
    # Get the response from User to Play Again    
    ans = input("Do you want to play again ? (Y/N) > ") 
  
    # Check the response from User and continue the loop
    # Otherwise break the loop to close the game
    if (ans == 'n' or ans == 'N') : 
        break
    
    
# Print a Thanks Message to the user
print("\nThanks for playing Rock Paper Scissor Game \n") 




"""
# importing time module 
import time 
  
def forsk(): 
    start_time = time.time()
    number = 0
    
    while number < 20:
        number = number + 1
   
    end_time = time.time() 
    print("forsk() function takes", end_time - start_time, "seconds") 
  
# Calling gfg 
forsk() 







# importing cProfile 
import cProfile 

def forsk(): 
    number = 0
    while number < 20:
        number = number + 1
        
cProfile.run('forsk()') 




#how to know current working directory


import os
os.getcwd()

"""









