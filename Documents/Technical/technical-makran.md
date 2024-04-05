# Game Technical Specification

## 1. Introduction
This document describes the technical specifications for the game Pizza Snake. It covers the system requirements, details of the game's architecture, technologies used, and key features of the game.

## 2 Hardware
- Macbook Pro 2020 I5 8th gen
- 8gb RAM
- 256gb SSD
## 3. Game Architecture
The game "Pizza Snake" is built using a custom game engine developed in C++17 and SFML. The architecture follows an Entity-Component-System (ECS) pattern. In this pattern, every object in the game is an Entity, which is composed of one or more Components. Systems manage the logic for each Component type.

- **Entities**: These are the game objects that exist within the game world. Examples include the player's snake, pizzas, and the game world boundaries.
- **Components**: These are simple data structures that are attached to entities. They contain state but no logic. Examples include Position, Velocity, and Renderable components.
- **Systems**: These contain the game logic and operate on entities that have specific components. Examples include a Movement System (which operates on entities with Position and Velocity components) and a Rendering System (which operates on entities with a Renderable component).

## 4. Technologies Used
- **Programming Language**: C++. This is a powerful language that provides high performance and fine control over system resources.
- **Game Engine**: Custom game engine developed in C++17 and SFML. This engine is specifically tailored for the needs of the "Pizza Snake" game.
- **Version Control**: GitHub. This is used for source code management, allowing multiple developers to work on the project simultaneously and keep track of changes.
- **IDE**: Visual Studio Code. This is the primary tool used for writing and editing the game's code.
- **Graphics**: Pixel Art. This is the art style of the game, which gives it a retro, arcade-like look.

## 5. Key Features
- **Snake Growth**: As the player's snake eats pizzas, it grows longer, increasing the difficulty of the game.
- **Food Consumption**: The player's snake can eat food to increase its length and score.
- **Random Food Display**: Food items are randomly displayed throughout the game area, providing a dynamic gameplay experience.
- **Scoring System**: Each food item consumed by the snake equals one score point.
- **Collision Detection**: The game detects collisions between the snake and the game boundaries or the snake's own body, triggering a game over.
- **Death Condition**: The game ends when the snake collides with the game boundaries or its own body.
- **Game Over Menu**: When the game ends, a game over menu is displayed with options to restart the game or exit.
- **Main Menu**: The game features a main menu where players can start the game, view high scores, or exit the game.
- **Pause Feature**: Players can pause the game at any time, allowing them to resume gameplay at their convenience.


## 6. Conclusion