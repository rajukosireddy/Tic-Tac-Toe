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
3. Checking for a Winner:

   ```bash
   def check_winner(board, player):
    winning_combinations = [
        [0, 1, 2], [3, 4, 5], [6, 7, 8],
        [0, 3, 6], [1, 4, 7], [2, 5, 8],
        [0, 4, 8], [2, 4, 6]
    ]
    for combo in winning_combinations:
        if all(board[i] == player for i in combo):
            return True
    return False
    ```
This function checks if the game board is full, indicating a draw.

4.Checking for a Draw:
   ```bash
   def is_board_full(board):
    return all(cell != '-' for cell in board)
   ```
This function checks if the game board is full, indicating a draw.

5. Minimax Algorithm with Alpha-Beta Pruning:
   ```bash
   def minimax_alpha_beta(board, depth, alpha, beta, maximizing_player):
   ```
This function implements the minimax algorithm with alpha-beta pruning for the AI's decision-making.

6. Finding the Best Move for AI:
   ```bash
   def find_best_move(board):
    ```
This function iterates through all possible moves and uses the minimax algorithm to find the best move for the AI.

7. Game Loop:
   ```bash
   while True:
    ```
The game loop allows players to take turns making moves until there is a winner or a draw.

8. User Input and Game Logic:
   ```bash
   move = int(input("select your choice(0-8): "))
   if board[move] == '-':
   ```
Takes user input for their move and implements the game logic for player and AI turns.

9. Printing Game Outcome:
    ```bash
    print("You win!")
   print("AI wins!")
   print("It's a draw!")
    ```
Prints the outcome of the game based on whether the player wins, the AI wins, or it's a draw.

    



   
   

   
