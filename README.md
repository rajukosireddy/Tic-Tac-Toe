# Tic-Tac-Toe Game


This is a simple implementation of the classic Tic Tac Toe game in Python.

## Table of Contents

- [Introduction](#introduction)
- [How to Play](#how-to-play)
- [Features](#features)
- [Implementation Details](#implementation-details)
- [Run the Game](#run-the-game)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Welcome to the Tic Tac Toe game! This Python program allows you to play Tic Tac Toe against an AI opponent. The game employs the minimax algorithm with alpha-beta pruning for intelligent AI moves.

## How to Play

1. The game is played on a 3x3 grid.
2. You (X) play against the AI (O).
3. Choose a cell to make your move by entering a number from 0 to 8.
4. The game continues until there is a winner or a draw.

## Features

- Player vs. AI gameplay.
- Intelligent AI moves using the minimax algorithm with alpha-beta pruning.
- Interactive command-line interface.

## Implementation Details

The main logic of the game is implemented in the `minimax_alpha_beta` function. This function utilizes the minimax algorithm with alpha-beta pruning to make optimal AI decisions.

## Run the Game

To run the game, follow these steps:
1. Game Initialization:
   ```bash
   board = ['-'] * 9
   AI = 'O'
   YOU = 'X'
   ```
   
1. The game board is represented as a list with 9 elements, initially filled with dashes (-).
2. The AI is represented by the symbol 'O', and the player (YOU) by 'X'.

2.Printing the Board:
  ```bash
      def print_board(board):
    for i in range(0, 9, 3):
        print(board[i] + '|' + board[i + 1] + '|' + board[i + 2])
    print()
```


   
