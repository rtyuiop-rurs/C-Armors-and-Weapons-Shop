🛒 Weapons & Armor Shop (C++)

This is a small C++ console program where the player can buy weapons and armor from a shop.
The player starts with some random gold and can choose which items to buy as long as they have enough money.


Features
Random Gold Allocation: Each customer starts with 100-200 gold

Armor Shop: Purchase from 5 different armor types (Copper, Iron, Gold, Diamond, Netherite)

Weapon Shop: Purchase various weapons (implementation details in code)

Inventory Management: Track purchased items and remaining gold

Input Validation: Robust error handling for user inputs

Program Structure
Core Components
Armor System
cpp
namespace Armor {
    enum armor { copper, iron, gold, diamond, netherite, armor_count };
    // Associated costs and string representations
}
Customer Class
Attributes: Name, gold balance, shopping cart

Methods: Purchase items, check inventory, get gold balance

Shop Interfaces
armorShop(): Armor purchasing interface

weaponShop(): Weapon purchasing interface

buyArmor()/: Individual item purchase logic

How to Use
Compilation: Ensure you have the "Random.h" header file

Run the program

Enter your name when prompted

View available items and their costs

Purchase items by entering the corresponding number

Type 'q' to exit the shop

View final inventory and remaining gold

Controls
Number keys (0-4): Select corresponding armor/weapon

'q' key: Quit the current shop

Invalid inputs: Automatically handled with error messages

Item Costs
Copper Armor: 30 gold

Iron Armor: 40 gold

Gold Armor: 50 gold

Diamond Armor: 66 gold

Netherite Armor: 78 gold

Weapon costs: Defined in Weapon namespace


Example Output
text
Enter your name: Alice
Hello Alice You have 150 amount of gold
Here is the armor sets for today: 
0) copper armor costs: 30
1) iron armor costs: 40
...
You bought iron armor and you have: 110 left
Inventory:
Armor bought: iron set x1
The amount of gold left is: 110

Notes
Gold is randomly allocated between 100-200 at customer creation

Players cannot purchase items they cannot afford

Inventory only shows items with quantity > 0

Program handles invalid inputs gracefully
