# snake-ladder
 A snake-ladder game along  is constructed in c language
I.The <time. h>header file contains definitions of functions to get and manipulate date and time information
II.We create a function called rollDice() to imitate the action of rolling a die with six sides.
   The playTurn() function represents a player's turn, which involves rolling the dice, adjusting the player's position and managing any encounters with snakes and ladders.
   We establish the locations of both snakes and ladders, along with their respective endpoints.
   Within the main() function, we take turns between players and invoke playTurn() until one of them reaches or surpasses position 100.
let's breakdown the program into simpler steps:

1.Include Header Files:
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
These lines include the necessary header files for input/output, random number generation, and time functions.

2.rollDice Function:
int rollDice() {
    return rand() % 6 + 1;
}
This function generates a random number between 1 and 6 to simulate rolling a dice.
rand() generates a random integer, and % 6 restricts it to the range [0, 5]. Adding 1 ensures it's in the range [1, 6].

3.updatePosition Function:
This function updates a player's position based on their current position and the result of their dice roll.
It also checks for snakes and ladders on the board and adjusts the position accordingly.

4.Main Function:
It seeds the random number generator using the current time to ensure different random numbers on each run.
Initialize player positions (player1Position and player2Position) and currentPlayer to start with Player 1.
Display a welcome message.

5.Game Loop:
The game loop continues until one of the players reaches or exceeds position 100.

6.Player Turn:
It prints the current player's turn and the result of their dice roll.

7.Update Player's Position:
Depending on the current player, it updates their position using the updatePosition function.
It prints the new position of the player.

8.Check for Win:
After each turn, it checks if a player has reached position 100, indicating a win.

9.Switch Players:
It switches the current player for the next turn.
Finally, the program returns 0 to indicate successful execution and terminates.

This program simulates a basic Snake and Ladder game for two players and displays the game's progress and outcome. 
