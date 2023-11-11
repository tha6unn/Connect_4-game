# Connect_4-game
•	Connect Four (also known as Connect 4, Four Up, Plot Four, Find Four, Captain's Mistress, Four in a Row, Drop Four) is a two-player connection rack game.

•	In which the players choose a color and then take turns dropping colored tokens into a seven-column, six-row vertically suspended grid.

•	The pieces fall straight down, occupying the lowest available space within the column. The objective of the game is to be the first to form a horizontal, vertical, or diagonal line of four of one's own tokens.

•	Here, the player enters a column number to place their respective token. The token is placed at the bottom most empty cell in that column.

2.	MODULES DESCRIPTION



Connect4 Class: This is the main module that encapsulates the game logic. It includes private member variables like the game board (board) and the current player (“currentPlayer”), as well as public member functions for various operations related to the game.

Constructor: The constructor initializes the game board by setting all positions to empty spaces (' ') and sets the currentPlayer to 1 (player 1). It ensures that the game starts with an empty board and assigns the first turn to player 1.

Display Board: The displayBoard() function is responsible for printing the current state of the game board to the console. It iterates through the board array and displays each cell, resulting in a visual representation of the game board.

Make Move: The makeMove() function allows a player to make a move by specifying the column where they want to drop their disc. It validates the move by checking if the column number is within the valid range and if the selected column has available space. If the move is valid, it updates the board array with the player's disc and returns true. Otherwise, it displays an error message and returns false.

Check Win: The checkWin() function examines the game board to determine if the current player has achieved a winning position. It checks for four connected discs horizontally, vertically, and diagonally. If a winning configuration is found, it returns true; otherwise, it returns false.

Switch Player: The switchPlayer() function updates the currentPlayer variable to switch to the next player's turn. If the current player is 1, it changes it to 2, and vice versa.

Play Game: The playGame() function controls the main game loop. It displays the game board, prompts the current player for a move by inputting a column number, and makes the move using the makeMove() function. If a player wins, it displays the winning message and ends the game. Otherwise, it switches to the next player's turn and continues the loop until a win condition is met.

Main Function: The main() function acts as the entry point of the program. It creates an instance of the Connect4 class, initializes the game, and starts playing by calling the playGame() function.
