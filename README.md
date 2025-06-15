🐍 Overview of Snake Game in Python
The Snake Game is a well-known classic arcade game. The player controls a snake that grows in size every time it eats food. The game ends if the snake collides with the wall or itself.

This game is built using Python's pygame library, which is used for creating 2D games.

🔍 Explanation of Code – Theoretical View
1. Pygame Initialization
The pygame.init() function initializes all the modules required for pygame.

The game screen is created using pygame.display.set_mode().

Fonts and clock (for controlling game speed) are also initialized.

2. Color and Screen Setup
Several color variables are defined using RGB values (like white, black, red, green).

The game window size (width and height) is set.

3. Snake Structure
The snake is represented as a list of coordinates.

Each block of the snake is 10x10 pixels.

A function is used to draw each block of the snake on the screen.

4. Food Generation
Food appears at a random location on the screen.

The food's position is adjusted to align with the snake's block size to ensure easy collision detection.

5. Movement and Controls
The snake's direction is controlled using the arrow keys.

The x and y position of the snake's head changes based on the key pressed.

6. Game Loop
The main loop runs until the player quits or loses.

In each iteration:

The snake's head moves.

The screen is updated.

Collision with food or wall is checked.

The snake grows if it eats the food.

The game ends if the snake hits the wall or itself.

7. Collision Detection
Wall collision: If the snake's head goes outside the screen boundaries.

Self collision: If the head's position matches any part of its body.

8. Score System
The score is calculated as the length of the snake minus 1.

The score is displayed on the screen continuously.

9. Game Over Handling
When the snake crashes, a message is displayed asking the user to:

Press Q to quit

Press C to restart the game

The game resets or exits based on the user’s input.

📌 Summary
The game uses a continuous loop to animate the snake.

Arrow keys control the direction.

Food is randomly placed.

Collision detection ends the game.

The game uses basic pygame functions like drawing shapes, handling events, and updating the screen.
