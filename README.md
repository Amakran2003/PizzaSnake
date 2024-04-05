# 2D Snake Game

## A simple game created using C++ and SFML
---
### What it looks like?

### This game has multiple states

- Main Menu State - Displays main menu
- Game Play State - The actual game play
- Pause Game State - Pause screen
- Game Over State - Displays game over screen

### Features

- Snake can be controlled with arrow keys
- Snake automatically advances 16px
- Food gets randomly placed
- Snake can eat food to grow in length
- Each food increase player score by 1 point

### Build Instructions

- Requirements
  - C++ compiler
  - Make
  - SFML lib
- Just run make command to generate the executable


### How to run the game?

macOS, Windows and Linux

On Vscode terminal or either your OS terminal 

- Go in the directory file by using `cd`
- First type `make` or copy and paste that:
```bash
g++ -Wall -Wextra -Wno-unused-parameter -std=c++17 -ggdb -Iinclude -Llib src/AssetMan.cpp src/Game.cpp src/GameOver.cpp src/GamePlay.cpp src/MainMenu.cpp src/PauseGame.cpp src/Snake.cpp src/StateMan.cpp src/main.cpp -o bin/main -lsfml-graphics -lsfml-window -lsfml-system
```
- Finally type `bin/main`
Enjoy!
