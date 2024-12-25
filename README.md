### download the ZIP file \ Everthing should be in there

# Puzzle Game Maker
Overview :
Welcome to the Puzzle Game! This game allows you to create your own custom puzzle levels using a built-in Tilemap Maker. The game itself is designed so that all objects and tiles are hard-coded, so you only need to focus on creating your own levels by arranging tiles and saving the map data in a JSON format.


# How to Create and Integrate Maps
Use the Tilemap Maker
The game provides a Tilemap Maker that allows you to design your own puzzle maps. The Tilemap Maker has a user-friendly interface for selecting and placing tiles, which represent different elements in the game world (such as walls, floors, obstacles, etc.).

# Saving the Map
Once you've designed your map, save it in the JSON format. The Tilemap Maker will automatically generate this JSON file based on your map design.

# Integrating the Map into the Game
To use your custom map in the game
Open the saved JSON map file from that will now appear in your direcotry named "saved_map.txt" 
Copy the contents of the JSON file.
Paste the JSON data into the map section of the game’s code.(Puzzle_Game_Maps)
Ensure the map is properly placed in the designated map variable or array within the game's code.
Hard-Coded Objects and Tiles
The game’s objects and tiles (such as player characters, enemies, interactive objects, and backgrounds) are all hard-coded into the game. This means you do not need to create or modify them yourself. You just need to design the layout of the map using the Tilemap Maker.

# Running the Game
After integrating your custom map, simply run the game to test your new puzzle level. The game will automatically load the map from the code and display it in the game world.

# Important Notes
The tile types and objects used in the Tilemap Maker correspond to hard-coded values in the game, so make sure to use the correct tile types when designing your maps.
If you need to adjust the layout of tiles or objects, you can do so by modifying the map in the Tilemap Maker and re-saving the JSON file.

Tile Map Maker will only save on map file at a time so make new one and savig will overright old one so make sure you have already copy and paste it into the maps.

 # Files
 Make sure everthong is in th same Directory and make sure you have the Assets fold with all the grapics in it , the Assets folder holds everthing for the game and tile map maker 

# Puzzle Game OverView
This is a simple Puzzle Game built using Pygame, where players navigate a character through various puzzle levels. The game supports custom levels, basic player interaction, and a particle system for effects. The game includes multiple levels, inventory management (coins and keys), and a rating system based on player performance.

## Key Features
Multiple Levels: Navigate through different puzzle maps, each with unique obstacles and challenges.
Player Interaction: Players can interact with tiles to collect items (coins, keys) or trigger events.
Particle Effects: Visual effects such as explosions or animations when interacting with the game world.
Game State Management: Track progress across multiple levels with a star rating system, based on coins collected and deaths.
Dev Mode: The developer mode enables level navigation (previous/next levels) during gameplay.
Libraries Used
pygame: A popular library used to create video games with Python.
random: For randomization of certain events or behaviors in the game.
itertools: To create more complex patterns or combinations within the game logic.
time: For handling timing-related events, such as pauses and frame rates.
Game Structure
The game is structured with multiple modules that handle different aspects of the game logic:

### Main Script: game.py
The primary file that runs the game. It sets up the Pygame window, initializes game states, loads assets, and contains the main game loop.

### Maps:
Maps are defined and handled in the Puzzle_Game_Maps module. Each level is represented as a function (e.g., Starting_Map, Map_1, Map_2, etc.), and they return a tilemap layout when called.

### Player: Puzzle_Game_Player.py
Handles player movement and interactions with the map. The move_player function moves the player based on user input, while interact_with_tile checks for interactions with tiles (e.g., collecting items, triggering events).

### Particle System: Puzzle_Game_Particle_System.py
Responsible for generating and rendering particles to create visual effects like explosions or animations when events occur.

### Screens and UI: Puzzle_Game_Screens.py
Includes functions to display messages (e.g., "Stage Complete", "Game Over") and show the player's inventory status (coins, keys, deaths).

## Dev Mode
DEV_MODE: If enabled, allows the player to move between levels using the Q and E keys.

## Game Logic
The game progresses through different maps, with the player's goal being to collect all the coins while avoiding death. The CalculateStarRating function determines the player's performance, giving 3 stars for a perfect run (no deaths and all coins collected), 2 stars for all coins but some deaths, and 1 star for incomplete runs.

## Key Functions
RunPuzzleGame: Initializes the game and runs the main game loop.
ResetGameState: Resets the game state (e.g., player position, inventory, map, etc.) after a death or level transition.
UpdateMovingObjects: Updates the position and direction of any moving objects in the game world.
interact_with_tile: Handles interactions with tiles like picking up coins, opening doors with keys, etc.
GenerateParticles and RenderParticles: Handle the creation and rendering of visual effects such as particles when the player interacts with objects in the game world.
DisplayMessage: Shows messages like "Stage Complete" or "Game Over" along with the player's performance rating.

### Assets
The game loads images and sounds stored in the assets directory, including player and item sprites, sound effects, and background music.

### Tilemap System
Levels are designed using a grid-based tilemap system where each map is represented as a grid of tiles. Moving objects, like enemies or obstacles, are represented with specific values in the tilemap, and their movement is updated each fram
