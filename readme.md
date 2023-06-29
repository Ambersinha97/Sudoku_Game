# Installing or running java application
1. First go to release section on github repository then
2. Install SudokuSetup.exe file on your machine to run the application.
   

# Introduction of Project

1. This is the introductory session of a minor project called Sudoku Solver.
2. The project is a game that allows the user to solve Sudoku puzzles.
3. The aim of the project is to recreate the experience of solving Sudoku puzzles that people used to do in newspapers.
4. The game consists of a 9x9 grid of boxes that can be filled with digits from 1 to 9.
5. The game has a reset button, an exit button, a solution button, and a check moves button.
6. The reset button empties the whole grid, the exit button closes the execution, the solution button fills the grid with expected solutions, and the check moves button checks whether the move is correct or not.
7. The game grid consists of 9 rows and 9 columns, which are buttons that can be clicked to fill the digit in the box.
8. The project primarily uses Java language for coding with Maven.
9. Java Swing is also used to build the GUI application.
10. Java Swing is a part of JFC (Java Foundation Classes) which is used to create window-based applications.
11. AWT (Abstract Windowing Toolkit) is the base for Java Swing.
12. Java Swing provides a lot of styling components such as buttons, labels, text fields, etc. for building the GUI.
13. JFrames are top-level containers provided by Java Swing which provide a playground for designing components.
14. JFrames are also known as base windows on which other components such as menu bars, panels, labels, text fields, buttons, etc. rely.
15. Almost every Java Swing application starts with the JFrame window.

# Steps used to build this Project.

1. The main Jframe form is used for designing.
2. The size of the Jframe is set to 500x630.
3. Nine grids is added to the Jframe using a panel for each grid.
4. Each panel is resized to 146x149.
5. Panels is copied and pasted to adjacent places.
6. Line borders is then added to each grid.
7. Buttons is added to each grid and resized according to the grid size.
8. All buttons are added before further adjustments are made.
9. 9 buttons are present in every grid, with each button named according to row and column.
10. The buttons for selection, reset, exit, OK solution, and check moves are present, with their names changed, and size set to 40.
11. A 2D array string is created to store the solver values of Sudoku.
12. The turn variable stores the value of the selection button that is pressed.
13. The value of the turn variable will set in the clicked grid.
14. The code for button functionalities is demonstrated for a few buttons, where an empty button will take the value of the turn variable and the background will be set to white.
15. For already filled buttons, a warning message box will appear.
16. The message inside the box can be customized according to need.
17. Upon clicking the exit button, a warning method will be displayed with two options: Yes or No. If Yes is clicked, the program will stop the execution and the JFrame window will be closed.
18. Upon clicking the reset button, a warning box will be displayed using JOptionPane. If Yes is clicked, the program will reset by replacing the prefilled grids with a blank text.
19. The function 'reset game' is called upon clicking the reset button. The 'buttons' array stores the names of the 81 buttons, while the 'predefined buttons' array stores the names of the buttons that are predefined.
20. Nested for loops are used to iterate over the 9 grids and their 9 buttons. A boolean flag variable is used to identify whether the value of a specific grid is predefined or not.
21. If a grid is not predefined, its value will be set to blank upon clicking the reset button.
22. The solution button function is designed to handle two arrays: the solved board and the current board. In the solution function, it checks whether a grid cell is already filled or not. If it's not filled, the function replaces the value with the corresponding value from the solved board array. On a click of the solution button, it displays all the solutions and then hides them based on a global flag that toggles between functionalities. When the flag is true, it shows the solutions and changes the button text to "Hide Solution"; when false, it hides the solutions and changes the button text to "See Solution". The button also uses a boolean flag to determine if it's predefined or not, replacing its value with the value from the solved board array for the same index. Additionally, the function sets the foreground and background color for the button accordingly.
23. The Check_Moves button function is designed to display the filled box is correct or not. If box is correct then change the background color to green and if not then change background to red color.
