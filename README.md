# snake-gun-water-Game
# SNAKE WATER GUN GAME
# if 1 so snake
# if -1 so water
# if 0 so gun
import random

computer =random.choice([1,-1,0])
youstr=input("Enter yout choice " )
youDict={"s":1,"w":-1,"g":0}
you=youDict[youstr]

reverseDict = {1:"snake",-1:"water",0:"Gun"}


print(f"You chose  {reverseDict[you]}\nComputerchoice {reverseDict[computer]}")
if(computer==you):
    print("its a draw")
else:
    if(computer==-1 and you ==1):
        print("u won by snake") 
    elif(computer ==-1 and you==0):
     print("you lose")   
    if(computer==1 and you ==-1):
     print("u lose by snake") 
    elif(computer ==1 and you==0):
        print("you win")
    if(computer==0 and you ==-1):
        print("u won by Water") 
    elif(computer ==0 and you==1):
        print("you lose by Gun")
    else:
       print("something went wrong")
