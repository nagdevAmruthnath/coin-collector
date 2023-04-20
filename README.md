# coin-collector

Coin Collector is a simple game built using Pygame, a popular Python library for game development. The game is played on a 2D plane, where the player must collect coins while avoiding obstacles. The game features progressively increasing difficulty as the player's score increases.

## Getting Started
To run the game, you must have Python 3.x installed on your computer. You can download the latest version of Python from the official website: https://www.python.org/downloads/

You must also install the Pygame library, which can be done by running the following command in your terminal or command prompt:
```
pip install pygame
```
Once you have installed Python and Pygame, you can run the game by executing the following command in your terminal or command prompt:

```
python game.py
```
## Gameplay
The player's character is placed at the bottom of the screen, and the game features two types of objects: coins and obstacles. Coins are circular objects that fall from the top of the screen and can be collected by the player. Obstacles are rectangular objects that move from top to bottom and can cause the player to lose if they collide with them. The game ends when the player collides with an obstacle.

The player moves the character left and right using the arrow keys to collect coins and avoid obstacles. Each time the player collects a coin, their score increases by one. The game becomes progressively harder as the player's score increases, with obstacles moving faster and appearing more frequently.

## Code Structure
The game is built using Pygame, which provides a set of modules and functions for creating games. The Pygame pygame.init() function is used to initialize the library, and pygame.display.set_mode() is used to create the game window. The game objects, including the player, coins, and obstacles, are initialized with their respective properties such as size, position, and speed. The player's movement is handled using the pygame.key.get_pressed() function, which returns the state of all keyboard keys. Collision detection is implemented using Pygame's pygame.sprite.spritecollide() function.

The game also features a background color, which is set to black, and a title displayed at the top of the screen using Pygame's font module. The game's score is also displayed on the screen using the pygame.font.SysFont() function to create a font object, and font.render() to render the score text onto a surface.
Contributing

If you're interested in contributing to the game, feel free to fork the repository and make your changes. You can also open an issue on GitHub if you encounter any bugs or have any suggestions for improvement.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.