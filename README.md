# Rock-Paper-Scissor

Explaination of the code:

1. Import Libraries:
   - `from tkinter import *`: Imports all classes, functions, and constants from the Tkinter library.
   - `import random`: Imports the random module for generating random computer choices.

2. Create the Tkinter Window:
   - `root = Tk()`: Creates the main Tkinter window object.

3. Set Window Properties:
   - `root.geometry("300x300")`: Sets the initial size of the window.
   - `root.title("Rock Paper Scissor Game")`: Sets the window title.

4. Define Computer Choices:
   - `computer_value`: A dictionary mapping integers 0, 1, 2 to corresponding choices (Rock, Paper, Scissor).

5. Game Functions:
   - `reset_game()`: Resets the game by enabling the buttons and clearing the result labels.
   - `button_disable()`: Disables the game buttons after a move.
   - `isrock()`, `ispaper()`, `isscissor()`: Functions corresponding to player choices, determining the winner against the computer's random choice.

6. Labels and Frames:
   - Labels for player choice (`l1`), versus text (`l2`), computer choice (`l3`), and match result (`l4`) are created.
   - A frame (`frame`) is used to organize the labels.
   - Another frame (`frame1`) is used for the game buttons.

7. Game Buttons:
   - Buttons (`b1`, `b2`, `b3`) for Rock, Paper, and Scissors are created within `frame1`.
   - Each button is associated with a specific player move function.

8. Reset Button:
   - `Button(root, text="Reset Game", font=10, fg="red", bg="black", command=reset_game)`: Creates a button to reset the game, associated with the `reset_game` function.

9. Execute Tkinter:
   - `root.mainloop()`: Starts the Tkinter event loop, allowing the GUI to be interactive.

In summary, the code creates a simple GUI for a Rock, Paper, Scissors game with buttons for player moves, labels to display choices and results, and a reset button to restart the game. The game logic is implemented through functions that compare player choices with randomly generated computer choices.
