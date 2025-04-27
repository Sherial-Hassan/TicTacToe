Tic-Tac-Toe with Minimax and Alpha-Beta Pruning 


1. Introduction
This project presents an intelligent Tic-Tac-Toe game developed using the Minimax algorithm and its optimized variant, Alpha-Beta Pruning, implemented in Python.
 The game features a user-friendly graphical interface where a human player competes against an AI that always plays optimally.
Key objectives of the project:
To understand and implement the Minimax algorithm.


To apply Alpha-Beta Pruning to enhance performance.


To integrate both algorithms into a GUI-based Tic-Tac-Toe game.


To compare the performance of basic Minimax and Alpha-Beta Pruning.



2. Algorithms Used
Minimax Algorithm
A recursive decision-making strategy for two-player games.


Explores all possible moves to determine the optimal choice.


Assumes the opponent plays optimally as well.


Time Complexity: O(b^d), where b is the branching factor and d is the depth of the tree.


Alpha-Beta Pruning
An optimization of the Minimax algorithm that prunes branches which do not affect the final decision.


Greatly reduces computational effort without affecting the outcome.


Best-case Time Complexity: O(b^(d/2)).



3. Code Structure
tictactoe_ai.py – Game Logic and AI
TicTacToe Class:
 Handles board state management, move validation, and win/draw detection.


AlphaBetaAI Class:
 Uses Minimax with Alpha-Beta Pruning to select optimal AI moves.


tictactoe_gui.py – Graphical User Interface (GUI)
Built using the Tkinter library.


Displays a 3x3 clickable grid.


Human plays as 'X', and the AI plays as 'O'.


Winner/draw messages are displayed through pop-up alerts.


The grid is colored, centered, and has a resizable layout.



4. GUI Features
Centered layout with a clean, minimalistic design.


Button colors:


'X' moves are highlighted in Blue.


'O' moves are highlighted in Green.


Responsive UI: the AI responds with a slight delay after the player’s move.


Board interaction is disabled automatically once the game concludes.



5. How the Game Works
The human player starts the game playing as 'X'.


After each player move, the AI calculates and executes the best possible move using Alpha-Beta Pruning.


After every move, the game checks for a win or a draw.


Upon a win or draw, a pop-up message is displayed, and no further moves can be made.



6. Minimax vs. Alpha-Beta Pruning (Performance Comparison)
Criteria
Minimax
Alpha-Beta Pruning
Nodes Explored
High
Significantly fewer
Speed
Slower
Faster
Optimal Move Selection
Yes
Yes
Efficiency (Depth > 4)
Low
Much better

Alpha-Beta Pruning drastically reduces the number of recursive calls while ensuring the same optimal results as the Minimax algorithm.

7. Requirements
Python 3.x installed.


Tkinter library (usually comes pre-installed with Python).


Run the tictactoe_gui.py file to launch the game.


