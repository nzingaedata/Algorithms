# Sudoku Solver

### Backtracking

Algorithmic-technique for solving problems recursively by trying to build a solution incrementally, one piece at a time, removing solutions that fail to satisfy the constraints of the problem at any point of time.

### Sudoku
Given a partially filled 9x9 2D array, the objective is to assign numbers from 1 to 9 to the empty cells so that every row, column, and subgrid of size 3x3 contains exactly one instance of the numbers from 1 to 9.

**Strategy**

We are trying to assign numbers one by one, whenever we find that the current number cannot lead to a solution, we remove it **(backtrack)** and try the next digit.

- **Step 1:** Find empty cells, get coordinates
- **Step 2:** Check row, col, subgrid of empty cell to see if number can be assigned
- **Step 3:** Assign number to cell
- **Step 4:** Repeat, until all numbers assigned to row
- **Step 5:**  If solution cannot be found remove number from cell and backtrack

**Rules**

- Grid Size: 9x9
- You cannot have the same number twice in a single row or column
- You cannot have the same number in the same 3x3 subgrid
- 1 <= num <= 9
