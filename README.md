# CS304-Tech-Writing-I3

OVERVIEW///
This is a program that implements a simple, multiplayer, tic-tac-toe game for the user to compete against each other with. This assignemnt was a lab I completed in my CS 232 class, where we were practiving with JPanel & action listeners. The object of the game is for one player to get 3 of either their "X"'s or "O"'s in a row first to win the game. The letter "X" is coorelated with the color red, and the letter "O" coorelates with the color blue. So you could perhaps try to get 3 of the same colors in a row to win the game.

INSTRUCTIONS///
-Once a player clicks the play button on the top of the Netbeans comiler.
-A new window will pop up showing a 3x3 grid on the user's screen
-Player 1 is X, so they will go first, then let player 2 go.
-Once a player succeeds in getting three of their colors in a row, they win!

METHODOLOGY///
-The program starts with JButton, where I make the board, which is essentially 9 buttons lined up in a 3x3 board for the user to click on to place their X or O.
-I then create an actionPerformed() function which takes in an event e, where if a player places their "piece" the button will make sure which player is going, and set that button to the specified color. This will happen until the winner is decided and it will call the displayWinner() function.
-The displayWinner() function also gives the player the option to restart the game with the "Play Again" button, or close the game with the "Close Button"
- It check to see if there is a winner, as well as that it check if there is a draw (where nobody has won the game). As well as make a function where the buttons (board) will reset after there is a winner or if there is a draw.
- The way I check for a winner if that I check all of the columns, rows, and diagonals to see if there are 3 of any of the same letter touching diagonally, vertically, or horizontally. All of these are done with the checkRows(), checkColumns(), and checkDiagonals() functions.
- Once all of these are checked, a winner is declared based on the results!

RESULTS///
- It is very significant for the players to see who has won the game for them to see who has come out victorious!

CONCLUSION///
- There is at least one error I am aware of by the time I am writing this. The players can place their color over the other player's color once it has already been placed. For example, blue can place their piece on a red's position once they have already placed it, causing confusion. I can definitely implement something which locks player 2from placing over player 1's square once they have placed their piece.
- I have learned a lot about action listeners and JFrame. This project really taught me a lot on how to think about every scenario possible in a simple game like tic-tac-toe.
