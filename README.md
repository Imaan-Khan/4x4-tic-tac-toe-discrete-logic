Project Overview
- Designed a 4×4 Tic-Tac-Toe game using discrete logic ICs  
- Implemented turn-based gameplay using flip-flops  
- Detected win and draw conditions using combinational logic  
- Simulated and verified the system in Proteus  

🔹Project Description

Tic-Tac-Toe is a two-player game where each player marks a grid with their symbol. In this implementation:

Player 1 is represented by Yellow LEDs (X)
Player 2 is represented by Red LEDs (O)

Players take turns selecting positions on a 4×4 grid, aiming to align four identical marks:

Horizontally
Vertically
Diagonally

This system is implemented entirely using digital logic ICs, without any microcontroller.

Players select grid positions using input switches. The system:

Enforces turn-based gameplay
Stores each move using memory elements
Continuously checks for winning conditions using logic circuits

A reset button is included to restart the game at any time.

The system is built using standard digital logic ICs and basic electronic components.

🔹 Major Components:
AND, OR, NOT, XOR gate ICs
Flip-flops / latches (for memory)
Decoders / encoders (for input selection)
LEDs (for displaying moves and results)
Push buttons (player inputs)
Resistors
Power supply

🔹Working Principle
1. Input Switch Network (Move Selection)
Each grid cell is controlled by a dedicated switch
Pressing a switch represents a move for that cell
Inputs are processed as binary signals
Logic ensures only valid moves are accepted
Once a cell is occupied, further inputs are ignored

2. Turn Control Circuit
Implemented using a flip-flop
Toggles after every valid move
Determines which player’s turn is active
Enables inputs only for the current player

3. Cell State Storage (Memory)
Each cell uses flip-flops to store its state
Once set, the value remains latched
Separate logic distinguishes between Player 1 and Player 2 moves

4. Win Detection Logic
Implemented using combinational logic circuits
All winning combinations are hardwired:
Rows
Columns
Diagonals
A win is detected when four cells align for the same player
Separate logic paths detect wins for each player

5. Game Locking Mechanism
Once a win is detected:
Inputs are disabled
No further moves can be made
Final state is preserved

6. Winner Indication (7-Segment Display)
Displays the result of the game
Logic encodes win signals into display outputs
Winning player shows ‘1’, losing player shows ‘0’
Output remains fixed after game completion








