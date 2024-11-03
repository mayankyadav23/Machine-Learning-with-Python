# Rock Paper Scissors Game 🎮

## Project Overview
This project is a Python implementation of the classic game Rock, Paper, Scissors, designed as part of the Machine Learning course on FreeCodeCamp. The objective is to create a player function that competes against four different bots, aiming to win at least 60% of the games in each match.

## Challenge Description
In this challenge, the player function receives the opponent's last move and must decide the next move ("R", "P", or "S") accordingly. The challenge encourages the implementation of strategies that adapt based on the opponent's play style.

## Files Included
- **RPS.py**: Contains the main player function that you will implement.
- **RPS_game.py**: This file contains the game logic and predefined bots. Do not modify this file.
- **main.py**: A script for testing your player function against the bots.
- **test_module.py**: Contains unit tests to validate your player function.

## Setup Instructions
1. Clone the repository or open it in your Gitpod environment.
2. Ensure Python 3.x is installed.

## How It Works
1. The `player` function in `RPS.py` is called with the last move of the opponent as an argument.
2. It must return the next move ("R", "P", or "S").
3. The `play` function in `main.py` allows you to test your player function against the bots by specifying the players and number of games.

## Usage
To test your player function, follow these steps:
1. Open `main.py`.
2. Uncomment the line at the end of the file to run the tests automatically.
3. Alternatively, you can call the `play` function directly:
   ```python
   from RPS_game import play
   from RPS import player
   
   play(player, quincy, 1000, verbose=True)
