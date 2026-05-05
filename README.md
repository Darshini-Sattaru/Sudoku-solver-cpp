# Sudoku Solver (C++)
An efficient Sudoku solver that utilizes **Recursive Backtracking** and **Coordinate Mapping** to solve complex 9 \times 9 grids. This project focuses on input safety and algorithmic efficiency.
## 🚀 Key Features
 * **Recursive Backtracking:** Uses a depth-first search (DFS) approach to fill empty cells and backtrack when it hits a dead end.
 * **Pre-Validation Engine:** Includes an isValidGrid function that checks the user's input for rule violations (duplicates) before the solver begins.
 * **Coordinate Mapping:** Implements specialized math (box / 3 * 3) to navigate and validate 3 \times 3 sub-grids.
 * **Clean Visuals:** Formatted console output that draws a clear Sudoku board with vertical and horizontal boundaries.
## 🧠 Core Logic Explained
### 1. The Solver (Backtracking)
The solver finds an empty location (a 0) and attempts to place numbers **1–9**.
 * **Success:** If solveSudoku returns true, the path is saved.
 * **Backtrack:** If a path leads to a dead end, the cell is reset to 0 and the program tries the next number.
### 2. Validation (isValidGrid)
To save processing time, the program acts as a **Security Guard**. It uses a **frequency array** (size 10) to ensure no number appears twice in the same row, column, or 3 \times 3 box.
### 3. Sub-Grid Navigation
The program "jumps" to the start of each of the nine 3 \times 3 boxes using these formulas:
 * **Start Row:** (box / 3) * 3
 * **Start Column:** (box % 3) * 3
## 🛠️ How to Use
 1. **Clone the Repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/sudoku-solver-cpp.git
   
   ```
 2. **Compile**
   ```bash
   g++ main.cpp -o solver
   
   ```
 3. **Run**
   ```bash
   ./solver
   
   ```
## 📂 Project Structure
 * main.cpp: Complete source code including validation and solver logic.
 * README.md: Project documentation and technical overview.

Author
​Darshini Sattaru
