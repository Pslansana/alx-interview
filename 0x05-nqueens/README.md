# 0x05. N Queens

## Table of Contents
- [Introduction](#introduction)
- [Concepts Needed](#concepts-needed)
- [Requirements](#requirements)
- [Usage](#usage)
- [Algorithm](#algorithm)
- [Additional Resources](#additional-resources)

## Introduction

The **N Queens** problem is a classic algorithmic challenge in computer science and mathematics, focusing on placing **N** non-attacking queens on an **N×N** chessboard. This project requires implementing a solution using the **backtracking** algorithm in **Python**. The goal is to find all possible ways to place **N** queens on the board so that no two queens threaten each other. 

The project emphasizes recursion, backtracking, and Python list manipulation, providing a solid foundation for algorithmic thinking and problem-solving.

## Concepts Needed

To complete this project, you should be familiar with the following concepts:

### Backtracking Algorithms
Backtracking is a systematic way to explore all potential configurations of a problem. In this context, it helps to:
- Place a queen in a position
- Check if it's a valid position
- Recursively attempt to place subsequent queens
- Backtrack if a configuration does not lead to a solution

### Recursion
Recursive functions are used to implement the backtracking logic, enabling the algorithm to move step-by-step through the chessboard.

### List Manipulation in Python
Lists are used to store and track the queens' positions on the board. Manipulating lists correctly is crucial to maintain the current board state.

### Python Command Line Arguments
To take input dynamically, the program should be able to handle command-line arguments using the `sys` module. This allows specifying the board size **N** as an argument.

## Requirements

- Implement the N Queens solution in Python (Python 3 recommended).
- The program should handle input via command-line arguments, where **N** is passed as the board size.
- Only consider solutions where **N** queens are placed on the board without threatening each other.

## Usage

Run the program with **N** as the argument to specify the size of the chessboard. For example:

```bash
python3 n_queens.py 4

