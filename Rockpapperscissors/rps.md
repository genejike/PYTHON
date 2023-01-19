### import random module
`import random`

`rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''`

`paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''`

`scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''`

#Write your code below this line 👇
#import random

#input 
### put the ascii characters in a list to help call them easily
gameimages=[rock ,paper ,scissors]
### write out the input statement
person_pick = int(input("what do you choose?.0 for Rock,1 for paper and 2 for scissors.\n"))
if person_pick >=3 or person_pick < 0:
  print("you typed an invalid number!.you lose!")
else:
  print(gameimages[person_pick])
  computer_choice=random.randint(0 ,2)
  print(f"compute chooses:\n{gameimages[computer_choice]}")
  if person_pick ==0 and computer_choice == 2:
    print("you win!")
  elif person_pick == 2 and computer_choice == 1 :
    print("you win!")
  elif person_pick == 1 and computer_choice == 0:
    print("you win!")
  elif person_pick == computer_choice:
    print ("its a tie")
  else:
    print("you lose!" )
