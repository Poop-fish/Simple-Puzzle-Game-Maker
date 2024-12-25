# Puzzle Game Maker
Overview
Welcome to the Puzzle Game! This game allows you to create your own custom puzzle levels using a built-in Tilemap Maker. The game itself is designed so that all objects and tiles are hard-coded, so you only need to focus on creating your own levels by arranging tiles and saving the map data in a JSON format.

How to Create and Integrate Maps
Use the Tilemap Maker
The game provides a Tilemap Maker that allows you to design your own puzzle maps. The Tilemap Maker has a user-friendly interface for selecting and placing tiles, which represent different elements in the game world (such as walls, floors, obstacles, etc.).

Saving the Map
Once you've designed your map, save it in the JSON format. The Tilemap Maker will automatically generate this JSON file based on your map design.

Integrating the Map into the Game
To use your custom map in the game:

Open the saved JSON map file from the Tilemap Maker.
Copy the contents of the JSON file.
Paste the JSON data into the map section of the game’s code.
Ensure the map is properly placed in the designated map variable or array within the game's code.
Hard-Coded Objects and Tiles
The game’s objects and tiles (such as player characters, enemies, interactive objects, and backgrounds) are all hard-coded into the game. This means you do not need to create or modify them yourself. You just need to design the layout of the map using the Tilemap Maker.

Running the Game
After integrating your custom map, simply run the game to test your new puzzle level. The game will automatically load the map from the code and display it in the game world.

Important Notes
The tile types and objects used in the Tilemap Maker correspond to hard-coded values in the game, so make sure to use the correct tile types when designing your maps.
If you need to adjust the layout of tiles or objects, you can do so by modifying the map in the Tilemap Maker and re-saving the JSON file.
Each map should be saved with a unique name to avoid overwriting previous maps when integrating them into the game.
