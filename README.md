# Snake-Game-in-C-
This code is a C++ implementation of a simple Snake game using the console. The game allows the player to control a snake that moves around the console, consuming fruits to increase its length and score while avoiding collisions with walls and itself. The game includes features like setting difficulty levels and saving scores to a file.

Here's a breakdown of the key components and functions in the code:

SnakeGame Class: This class encapsulates the entire game logic.

Private Member Variables: The class contains various member variables to track the game state, snake position, fruit position, score, tail segments, and game speed.

Enum Direction: An enum is used to represent different directions (STOP, LEFT, RIGHT, UP, DOWN) for the snake movement.

Constructor: The constructor initializes the game's parameters, such as width, height, and initial positions.

SetDifficulty Function: This function sets the game speed based on the selected difficulty level.

Draw Function: Draws the game elements on the console, including the snake, fruit, and walls.

Input Function: Handles keyboard input to change the snake's direction.

Logic Function: Updates the game logic in each iteration. It moves the snake, checks for collisions, updates the tail segments, and handles fruit consumption.

SaveScore Function: Saves the player's score to a text file.

Play Function: The main game loop where the game is played. It repeatedly calls functions to draw, take input, and update logic. It also controls the game speed using the Sleep function.

main Function: The entry point of the program.

It gets the difficulty level from the user.

Creates an instance of the SnakeGame class and sets the difficulty level.

Calls the Play function to start the game loop.

Control Keys:

'j': Move left
'l': Move right
'i': Move up
'k': Move down
'x': Quit the game
Console Output: The game's visuals are displayed in the console window. The snake's body is represented by 'o', the snake's head by 'O', and the fruit by 'F'. Walls are represented by '#'.

Game Over: When the game is over (snake collides with walls or itself), the player's final score is displayed, and the score is saved to the "scores.txt" file.
