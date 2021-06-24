import pyautogui, pyperclip, random, time

print("Tool spam 1.0 by Axeyed")

msg = input("enter content to spam:").split(" || ")

n = int(input( "enter spam count:" ))

m = float(input("Enter time delay:  "))

 

print("Start")

for i in range(5,0,-1):

                print(i,end="...",flush='True')

print("Starting")

 

for i in range(n):

                pyperclip.copy(random.choice(msg))

                pyautogui.hotkey("ctrl","v")

                pyautogui.press("enter")

time.sleep(m)
