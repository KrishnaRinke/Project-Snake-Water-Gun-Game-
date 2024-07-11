# Project-Snake-Water-Gun-Game-using python
import random

computer=random.choice([-1,1,0])

youstr=input("snake\nwater\ngun\nmake your choice:")
youDict={"snake":1,"water":-1,"gun":0}
reverseDict={1:"snake",-1:"water",0:"gun"}

you=youDict[youstr]

print(f"you choose {reverseDict[you]} and computer choose {reverseDict[computer]}")

if(computer==you):
    print("its a draw")
else:
    if(computer==-1 and you==1):
        print("congrats you win!")
    elif(computer==-1 and you==0):
        print("you loose \n better luck next time")
    elif(computer==1 and you==-1):
        print("you loose \n better luck next time")
    elif(computer==1 and you==0):
        print("congrats you win!")
    elif(computer==0 and you==1):
        print("you loose \n better luck next time")
    elif(computer==0 and you==-1):
        print("congrats you win!") 
    else:
        print("something went wrong")
        
         
