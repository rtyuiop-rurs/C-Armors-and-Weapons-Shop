# Armor & Weapon Shop Simulator

## Description
A C++ console-based shopping simulation where players can purchase armor and weapons using randomly allocated gold.

## Features
- **Random Gold Allocation**: Each customer starts with 100-200 gold
- **Armor Shop**: Purchase from 5 different armor types (Copper, Iron, Gold, Diamond, Netherite)
- **Weapon Shop**: Purchase various weapons (implementation details in code)
- **Inventory Management**: Track purchased items and remaining gold
- **Input Validation**: Robust error handling for user inputs

## Program Structure

### Core Components

#### Armor System
```cpp
namespace Armor {
    enum armor { copper, iron, gold, diamond, netherite, armor_count };
    // Associated costs and string representations
}
```

#### Customer Class
- **Attributes**: Name, gold balance, shopping cart
- **Methods**: Purchase items, check inventory, get gold balance

#### Shop Interfaces
- `armorShop()`: Armor purchasing interface
- `weaponShop()`: Weapon purchasing interface  
- `buyArmor()`/: Individual item purchase logic

## How to Use

1. **Compilation**: Ensure you have the "Random.h" header file
2. **Run the program**
3. **Enter your name** when prompted
4. **View available items** and their costs
5. **Purchase items** by entering the corresponding number
6. **Type 'q'** to exit the shop
7. **View final inventory** and remaining gold

## Controls
- **Number keys (0-4)**: Select corresponding armor/weapon
- **'q' key**: Quit the current shop
- **Invalid inputs**: Automatically handled with error messages

## Item Costs
- Copper Armor: 30 gold
- Iron Armor: 40 gold  
- Gold Armor: 50 gold
- Diamond Armor: 66 gold
- Netherite Armor: 78 gold
- Weapon costs: Defined in Weapon namespace


## Example Output
```
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
```

## Notes
- Gold is randomly allocated between 100-200 at customer creation
- Players cannot purchase items they cannot afford
- Inventory only shows items with quantity > 0
- Program handles invalid inputs gracefully

## Future Enhancements
- Multiple shop types using template functions
- Enhanced inventory management
- Item selling functionality
- Persistent save/load system
