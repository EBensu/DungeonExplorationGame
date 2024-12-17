# Dungeon Exploration Game Explanation 
This game is basic dungeon adventure game written in C language.

--> Structs and Typedefs:
Defined for Statistics, Creature, Item, Player, Room, improving readability and reducing code complexity.
A macro limits the player's inventory to a maximum of 5 items.


-->Functions:
-createCreature: Creates creatures with health, strength, and an isAlive flag for game logic (e.g., passing a room or game over).

-getPlayerName: Gets the player’s name securely using fgets, with memory allocation to ensure accessibility outside the function.

-allocateString: Allocates memory for strings safely, preventing crashes due to insufficient memory.

-createItem: Creates items with properties like name, description, and effects on health/strength. Includes support for magic items.

-newRoom: Creates rooms with names, descriptions, directions, and associated items/creatures.

-connectRooms: Connects rooms bidirectionally for navigation.

-describeRoom: Provides detailed room descriptions, including items and creatures present.

-navigateRoom: Handles player movement between rooms based on user input.

-freeRoom and freePlayer: Release allocated memory after gameplay.

-look and inventory: Allow the player to inspect the current room and view their inventory.

-useItem: Uses an item from the inventory, boosting player stats and removing the item.

-attack: Implements combat with creatures, adjusting health/strength and handling game-over scenarios.

-saveGame and loadGame: Save and load game state to/from a file, including player and room information.

-pickupItemToInventory: Allows players to pick up items unless the inventory is full.

-->Main Method:
Initializes the player, rooms, creatures, and items.
Dynamically allocates memory and connects rooms.
Provides a menu-driven interface for user interaction.
Highlights:
Emphasis on memory safety (malloc, perror, strdup).
Secure input handling with fgets.
Modular design for future extensions like multiplayer mode, health restoration, and more complex game logic.
