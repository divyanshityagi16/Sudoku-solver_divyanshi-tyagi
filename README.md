# Sudoku-solver_divyanshi-tyagi
Sudoku Solver
Description
This project implements a Sudoku Solver using the backtracking algorithm. The solver takes a partially filled 9x9 Sudoku puzzle as input and returns a solved puzzle by filling in the empty cells while adhering to the rules of Sudoku.

Sudoku is a popular puzzle game where the goal is to fill a 9x9 grid with numbers from 1 to 9, ensuring that:

Each number appears only once in each row.
Each number appears only once in each column.
Each number appears only once in each of the nine 3x3 subgrids.
Features
Solves any valid Sudoku puzzle.
Implements the backtracking algorithm for efficient solution finding.
Handles edge cases like puzzles with no solution.
Outputs the solved puzzle or informs the user if no solution exists.
Technologies Used
Python 3.x: The entire implementation is written in Python, utilizing standard libraries and recursive functions.
Algorithm
The solver uses backtracking, a depth-first search technique:

Finds an empty cell in the puzzle.
Tries placing numbers from 1 to 9 and checks if they are valid.
Recursively attempts to solve the puzzle.
If a number leads to a valid solution, it proceeds; otherwise, it backtracks and tries another number.
How to Use
Clone or download the repository to your local machine.

bash
Copy
git clone https://github.com/yourusername/sudoku-solver.git
Open a terminal and navigate to the project folder.

Run the Python script:

bash
Copy
python sudoku_solver.py
The program will prompt you to enter the Sudoku puzzle row by row. Use 0 for empty cells.

After entering the puzzle, the program will solve it and print the solved puzzle.

Example Input:
plaintext
Copy
Enter the Sudoku puzzle row by row (use 0 for empty cells):
Row 1: 5 3 0 0 7 0 0 0 0
Row 2: 6 0 0 1 9 5 0 0 0
Row 3: 0 9 8 0 0 0 0 6 0
Row 4: 8 0 0 0 6 0 0 0 3
Row 5: 4 0 0 8 0 3 0 0 1
Row 6: 7 0 0 0 2 0 0 0 6
Row 7: 0 6 0 0 0 0 2 8 0
Row 8: 0 0 0 4 1 9 0 0 5
Row 9: 0 0 0 0 8 0 0 7 9
Example Output:
plaintext
Copy
Sudoku solved successfully!
5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
File Structure
bash
Copy
sudoku-solver/
├── sudoku_solver.py   # Python script for solving Sudoku
├── README.md          # This README file
└── example_input.txt  # Example Sudoku puzzle (optional)
Contributing
If you'd like to contribute to this project:

Fork the repository.
Create a new branch for your feature or bug fix.
Commit your changes and push them to your forked repository.
Open a pull request for review.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
The backtracking algorithm used in this project is a well-known method for solving constraint satisfaction problems, and it's the core of many puzzle-solving applications.
