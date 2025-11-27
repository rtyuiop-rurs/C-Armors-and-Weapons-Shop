# C-Armors-and-Weapons-Shop
This is a simple c++ console program that simulates a armors and weapons shop where user can buy either weapons and armor with a randomly generated gold value, And they can view their inventory. 

🛒 Weapons & Armor Shop (C++)

This is a small C++ console program where the player can buy weapons and armor from a shop.
The player starts with some random gold and can choose which items to buy as long as they have enough money.

This project is good practice for beginners who want to learn:

enums

arrays

classes

basic input handling

simple game loops

⭐ What the Program Does

The player types their name.

The game gives the player a random amount of gold.

The player can visit:

The Armor Shop

The Weapon Shop

Each shop shows a list of items with their prices.

The player chooses what to buy by entering a number.

If the player has enough gold, the item is added to their inventory.

The player can quit the shops anytime.

When they exit, the game shows a final inventory summary.

🛡 Armor in the Game

Examples (depends on your code):

Copper armor

Iron armor

Gold armor

Diamond armor

Netherite armor

Each armor has a fixed cost.

⚔ Weapons in the Game

Examples:

Sword

Shield

Halberds

Hammer

Greatsword

Each weapon also has a fixed cost.

👤 Player Features

Starts with random gold

Can buy items

Cannot buy things they can't afford

Keeps track of how many items are bought

Inventory is shown at the end

🧰 How the Code Works (Simple Explanation)

Enums are used for item types (like armor names and weapon names).

std::array stores item names and their costs.

A class (Customer) stores:

gold

armor inventory

weapon inventory

Input is checked so the program doesn't break when the user types something wrong.

Functions handle:

buying items

showing shops

printing the final inventory

▶ How To Run the Program

If you're using g++:

g++ -std=c++20 -o shop shop.cpp
./shop
