# 🏴‍☠️ Treasure Island Adventure Game

Welcome to the **Treasure Island Adventure Game**! In this text-based adventure, you'll navigate through a series of choices to find hidden treasure. Choose wisely, as each decision can lead to victory or defeat!

---

## 📋 Features

- **Interactive Gameplay**: Make choices at critical junctures to progress through the story.
- **Multiple Endings**: Different outcomes based on the choices you make.
- **Simple Text Interface**: Engage with the game through easy-to-follow text prompts.

---

## 🔍 Code Overview

The game is structured using a series of conditional statements to guide the player through various paths based on their choices. Each decision point leads to a new set of options, ultimately resulting in either finding the treasure or facing an unfortunate end.

### Code Snippet

```python
print(''' 
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/[TomekK]
*******************************************************************************
''')

print("Welcome to Treasure Island!\nYour mission to find the treasure\n")
choice1 = input("You are at a cross road. Where do you want to go? Type 'left' or 'right'\n").lower()

if choice1 == 'left':
    choice2 = input("You have come to a lake, there is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across.").lower()

    if choice2 == "wait":
        choice3 = input("You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which color do you choose").lower()

        if choice3 == "red":
            print("It's a room full of fire. Game Over.")
        elif choice3 == "yellow":
            print("You found the treasure. You Win.")
        elif choice3 == "blue":
            print("You enter a room of beasts. Game Over.")
        else:
            print("You chose a door that doesn't exist. Game Over.")
    else:
        print("You got attacked by an angry trout. Game Over.")
    
else:
    print("Game Over!")
```

## 📋 Usage Instructions
1. Clone the Repository:
```bash
git clone https://github.com/your-username/treasure-island
cd treasure-island
```
2. Run the Game: Execute the script in a Python environment:
```bash
python treasure_island.py
```
3. Follow the Prompts:
  - Make choices by typing your responses as prompted.
  - Navigate through the story by choosing different paths.

## 🎮 Example Output
Example 1: Winning Scenario
```bash
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/[TomekK]
*******************************************************************************

Welcome to Treasure Island!
Your mission to find the treasure

You are at a cross road. Where do you want to go? Type 'left' or 'right'
left
You have come to a lake, there is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across.
wait
You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which color do you choose?
yellow
You found the treasure. You Win.
```
Example 2: Losing Scenario
```bash
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/[TomekK]
*******************************************************************************

Welcome to Treasure Island!
Your mission to find the treasure

You are at a cross road. Where do you want to go? Type 'left' or 'right'
left
You have come to a lake, there is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across.
swim
You got attacked by an angry trout. Game Over.
```

## ⚙️ Customization
Feel free to modify the code to include:
  - More paths and choices for a richer story.
  - Additional endings to enhance gameplay.
  - An interface for a more user-friendly experience.

## 📜 License
  This project is licensed under the MIT License. See the LICENSE file for details.

Enjoy your adventure on Treasure Island! 🗺️✨
