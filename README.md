# Pac-Man-like Game

Welcome to a Pac-Man-inspired game built using OpenGL and C++. In this game, you'll navigate through a maze collecting food while avoiding monsters. The goal is to collect as many points as possible without being caught!

## Features
- **Pac-Man Movement**: Navigate Pac-Man through the maze using the arrow keys.
- **Food Collection**: Collect food scattered throughout the maze to increase your points.
- **Monsters**: Avoid the monsters that roam the maze. If they catch you, the game ends.
- **Maze Design**: A customizable maze with obstacles and walls.
- **Simple Graphics**: Uses OpenGL for rendering the game environment and characters.

## Requirements

To run this game, you will need:
- A C++ compiler (such as GCC or MSVC)
- OpenGL and GLUT libraries installed

### Dependencies
- **GLUT**: A library for creating windows and handling user input for OpenGL programs.
- **OpenGL**: The graphics library used for rendering the game world.

### How to Install

1. **Install Dependencies**:
    - On Windows: Install the [FreeGLUT](https://www.transmissionzero.co.uk/software/freeglut-devel/) library.
    - On macOS: Install via Homebrew: `brew install freeglut`.
    - On Linux: Install using `sudo apt-get install freeglut3 freeglut3-dev`.

2. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/pacman-like-game.git
    cd pacman-like-game
    ```

3. **Compile the Code**:
    If you're using a terminal with the necessary libraries installed, you can compile the code with a command like:
    ```bash
    g++ -o pacman main.cpp -lGL -lGLU -lglut
    ```

4. **Run the Game**:
    After compiling, run the game with:
    ```bash
    ./pacman
    ```

## How to Play

- **Movement**: Use the arrow keys to move Pac-Man around the maze.
- **Objective**: Eat as much food as possible without being caught by the monsters.
- **Monsters**: They move randomly. If any monster touches Pac-Man, the game is over.
- **Points**: Each piece of food eaten will increase your score.

## Controls

- **Up Arrow**: Move Pac-Man Up
- **Down Arrow**: Move Pac-Man Down
- **Left Arrow**: Move Pac-Man Left
- **Right Arrow**: Move Pac-Man Right

## Game Logic

1. **Maze Layout**: The maze is constructed with walls, obstacles, and food scattered throughout. 
2. **Monster Movement**: The monsters will move randomly, avoiding walls and obstacles.
3. **Food Collection**: Pac-Man collects food by moving over it. Each food item gives points and is removed once eaten.
4. **Game Over**: If Pac-Man collides with a monster, the game ends. You can restart the game once it’s over.

## Code Structure

- **main.cpp**: The main game logic and rendering code.
- **init()**: Initializes the game settings, including OpenGL settings and game variables.
- **drawLaberynth()**: Draws the maze with obstacles and borders.
- **drawPacman()**: Renders Pac-Man on the screen.
- **drawMonster()**: Renders monsters on the screen.
- **keyPressed() & keyUp()**: Handle user inputs for Pac-Man movement.
- **updateMonster()**: Updates the monsters’ movement and behavior.

## Contributing

If you'd like to contribute to the project, feel free to fork the repository and create a pull request with your changes. Any improvements, bug fixes, or new features are welcome!

### To Contribute:
1. Fork the repo.
2. Create a new branch.
3. Commit your changes.
4. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The OpenGL and GLUT libraries for rendering.
- The inspiration from the classic Pac-Man game.
