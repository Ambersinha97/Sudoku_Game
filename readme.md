# Introduction of Project

This is the introductory session of a minor project called Sudoku Solver.
The project is a game that allows the user to solve Sudoku puzzles.
The aim of the project is to recreate the experience of solving Sudoku puzzles that people used to do in newspapers.
The game consists of a 9x9 grid of boxes that can be filled with digits from 1 to 9.
The game has a reset button, an exit button, a solution button, and a check moves button.
The reset button empties the whole grid, the exit button closes the execution, the solution button fills the grid with expected solutions, and the check moves button checks whether the move is correct or not.
The game grid consists of 9 rows and 9 columns, which are buttons that can be clicked to fill the digit in the box.
The project primarily uses Java language for coding with Maven.
Java Swing is also used to build the GUI application.
Java Swing is a part of JFC (Java Foundation Classes) which is used to create window-based applications.
AWT (Abstract Windowing Toolkit) is the base for Java Swing.
Java Swing provides a lot of styling components such as buttons, labels, text fields, etc. for building the GUI.
JFrames are top-level containers provided by Java Swing which provide a playground for designing components.
JFrames are also known as base windows on which other components such as menu bars, panels, labels, text fields, buttons, etc. rely.
Almost every Java Swing application starts with the JFrame window.

# Steps used to build this Project.

The main Jframe form is used for designing.
The size of the Jframe is set to 500x630.
Nine grids is added to the Jframe using a panel for each grid.
Each panel is resized to 146x149.
Panels is copied and pasted to adjacent places.
Line borders is then added to each grid.
Buttons is added to each grid and resized according to the grid size.
All buttons are added before further adjustments are made.
9 buttons are present in every grid, with each button named according to row and column.
The buttons for selection, reset, exit, OK solution, and check moves are present, with their names changed, and size set to 40.
A 2D array string is created to store the solver values of Sudoku.
The turn variable stores the value of the selection button that is pressed.
The value of the turn variable will set in the clicked grid.
The code for button functionalities is demonstrated for a few buttons, where an empty button will take the value of the turn variable and the background will be set to white.
For already filled buttons, a warning message box will appear.
The message inside the box can be customized according to need.
Upon clicking the exit button, a warning method will be displayed with two options: Yes or No. If Yes is clicked, the program will stop the execution and the JFrame window will be closed.
Upon clicking the reset button, a warning box will be displayed using JOptionPane. If Yes is clicked, the program will reset by replacing the prefilled grids with a blank text.
The function 'reset game' is called upon clicking the reset button. The 'buttons' array stores the names of the 81 buttons, while the 'predefined buttons' array stores the names of the buttons that are predefined.
Nested for loops are used to iterate over the 9 grids and their 9 buttons. A boolean flag variable is used to identify whether the value of a specific grid is predefined or not.
If a grid is not predefined, its value will be set to blank upon clicking the reset button.
The solution button function is designed to handle two arrays: the solved board and the current board. In the solution function, it checks whether a grid cell is already filled or not. If it's not filled, the function replaces the value with the corresponding value from the solved board array. On a click of the solution button, it displays all the solutions and then hides them based on a global flag that toggles between functionalities. When the flag is true, it shows the solutions and changes the button text to "Hide Solution"; when false, it hides the solutions and changes the button text to "See Solution". The button also uses a boolean flag to determine if it's predefined or not, replacing its value with the value from the solved board array for the same index. Additionally, the function sets the foreground and background color for the button accordingly.
The Check_Moves button function is designed to display the filled box is correct or not. If box is correct then change the background color to green and if not then change background to red color.