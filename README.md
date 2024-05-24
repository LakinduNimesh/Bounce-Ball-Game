# Bounce-Ball-Game

![Screenshot 2024-05-24 220455](https://github.com/LakinduNimesh/Bounce-Ball-Game/assets/149768006/4c662163-9fcb-45c8-a57b-297efdf135db)

# Bounce Ball Game

## Overview
This is a simple bounce ball game implemented in JavaScript. The objective of the game is to break all the bricks by hitting them with a ball that bounces off a paddle controlled by the player. The game features score tracking and game over/win conditions.

## Features
- Paddle controlled by mouse movements
- Dynamic ball movement
- Collision detection between ball and bricks
- Score tracking
- Game over and win conditions

## Installation

To run the game, you need a web browser that supports HTML5 Canvas and JavaScript.

### Steps
1. Clone the repository:
  
   [git clone](https://github.com/LakinduNimesh/Bounce-Ball-Game)
  
2. Open the `index.html` file in your web browser.

## Usage
- Move the paddle with your mouse to keep the ball in play.
- Break all the bricks to win the game.
- If the ball hits the bottom of the canvas without hitting the paddle, the game is over.

## Code Explanation

### Variables
- `canvas` and `ctx`: Used to set up the canvas and its 2D rendering context.
- `ballRadius`, `x`, `y`, `dx`, `dy`: Define the ball's properties and its movement.
- `paddleHeight`, `paddleWidth`, `paddleX`: Define the paddle's properties and its initial position.
- `rowCount`, `columnCount`, `brickWidth`, `brickHeight`, `brickPadding`, `topOffset`, `leftOffset`, `score`: Define the brick layout and the score.
- `bricks`: 2D array to store the brick objects with their properties.

### Functions
- `mouseMoveHandler(e)`: Updates paddle position based on mouse movement.
- `drawPaddle()`: Draws the paddle on the canvas.
- `drawBall()`: Draws the ball on the canvas.
- `drawBricks()`: Draws the bricks on the canvas.
- `trackScore()`: Displays the score on the canvas.
- `hitDetection()`: Detects collisions between the ball and bricks, updates the score, and checks for a win condition.
- `init()`: Main function to clear the canvas, redraw all elements, check for collisions, and update the ball's position.

### Game Loop
The game loop is set up using `setInterval(init, 10)`, which calls the `init` function every 10 milliseconds to update the game state and render the new frame.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests.
