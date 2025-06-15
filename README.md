# GAME-DEVELOPMENT-SNAKE-GAME #
*COMPANY*: CODTECH IT SOLUTIONS
*NAME*: MUDIT KUMAR
*INTERN ID*: CT04DF877
*DOMAIN*: C++ PROGRAMMING
*DURATION*: 4 WEEKS
*MENTOR*: NEELA SANTOSH KUMAR

##DESCRIPTION## 

✅ Game Output Description
🖥️ Window Setup
Window Title: "Snake Game"

Resolution: 800x600 pixels

Framerate Limit: 60 FPS

🐍 Gameplay
The snake starts at the center of the screen.

Movement begins when you press an arrow key.

The snake moves in a grid pattern of 20x20 pixel cells.

You control the snake with arrow keys:

↑ Up

↓ Down

← Left

→ Right

🍎 Food
A red circle randomly appears in a grid cell.

When the snake’s head reaches the food:

The snake grows by one segment.

The score increases by 1.

A "eat.wav" sound plays.

🧠 Score and Speed
Score is shown at the top-left corner.

The game gets faster as the score increases.

Speed is recalculated using:

cpp
Copy
Edit
speed = std::max(0.05f, 0.1f - score * 0.005f);
🎵 Audio
Background music (background.ogg) plays in a loop.

Eating food plays eat.wav.

Hitting the wall or yourself plays gameover.wav.

💀 Game Over
Occurs when:

The snake hits the edge of the window.

The snake collides with its own body.

"Game Over! Press R to Restart" is shown in red text centered in the window.

Press R to reset and restart the game.

🛠️ Requirements for Perfect Output
To get this perfect output, make sure you have:

✅ Assets in assets/ folder:
arial.ttf (font)

eat.wav (sound for eating)

gameover.wav (sound for collision)

background.ogg (looped music)

✅ SFML Libraries Installed and Linked:
Ensure your development environment is correctly linked with:

sfml-graphics

sfml-window

sfml-system

sfml-audio

✅ Compilation Example (Linux/g++):
bash
Copy
Edit
g++ snake_game.cpp -o snake_game -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
🎬 What You See and Hear
A green snake slithering around a black background.

A red circle (food) appearing in random places.

Score updating live in white text.

Sound effects and background music enhance immersion.

Snake grows and accelerates as you eat.

Game ends with sound and message if you crash.



🎮 Game Overview
In this game, the player controls a snake that moves around a grid-based field. The objective is to consume as much food as possible while avoiding collisions with the walls and the snake’s own body. Each time the snake eats food, it grows longer, making it harder to navigate without crashing. The game ends when the snake collides with itself or the boundaries of the screen (if wall collisions are enabled).

The game features:

Smooth movement and real-time updates

Dynamic growth as the snake eats food

Increasing difficulty as the snake gets longer

Simple and clear user interface

Responsive keyboard input

Restart and exit options after game over

🧰 Technologies Used
C++: The core programming language for game logic and system integration.

SFML (Simple and Fast Multimedia Library) / SDL (Simple DirectMedia Layer): Used for rendering graphics, handling user input, managing windows, and working with timers and textures.

Object-Oriented Programming: Structured design with classes such as Snake, Food, Game, and Renderer.

📦 Features & Implementation
🎨 Graphics & Rendering
Rendered in a 2D grid format with clear distinction between the snake, food, and background.

Frame rate and rendering loop managed via SFML/SDL clock utilities.

Double buffering to prevent flickering and ensure smooth transitions.

🐍 Snake Logic
Snake is implemented as a list or queue of segments (coordinates).

Movement logic updates the head position and shifts the body accordingly.

Growth is triggered upon collision with food, and the tail remains intact.

🍎 Food Generation
Randomly generated on the grid, ensuring it doesn't appear on top of the snake.

On consumption, food is re-spawned and the score is incremented.

💀 Collision Detection
Snake self-collision results in game over.

Optional edge wrapping or wall collision modes can be toggled in some versions.

🎮 Controls
Arrow keys (or WASD) to control direction.

Escape to pause or exit.

Spacebar or Enter to restart after game over.

📈 Learning Outcomes
This project is ideal for learning and demonstrating:

Game development principles in C++

Real-time input handling and rendering

Collision detection and grid-based logic

Object-oriented game architecture

Basic game loop implementation

Use of graphical libraries (SFML/SDL) for 2D development
