# Ruby Challenges / Sudoku Validator

## Exercise Intro

Difficulty: **Easy**

[Sudoku](http://en.wikipedia.org/wiki/Sudoku) is a logic-based combinatorial number-placement puzzle. The objective is to fill a 9×9 grid with digits so that each column, each row, and each of the nine 3×3 sub-grids that compose the grid contains all of the digits from 1 to 9.

Write a command-line program that can read a file containing a Sudoku grid and validates it. The grid can be partially or completely solved. Return either a  success message or a list of errors and their positions.

## Instructions

To start, you'll want to clone and run the setup script for the repo

    gh repo clone primaulia/sudoku-tester
    cd sudoku-tester
    bin/setup

A Sudoku is valid if:

1. It has no duplicates in a row
2. It has no duplicates in a column
3. It has no duplicates in a sub-group (the nine smaller 3x3 grids).

## Input files
The input files look like this

```
8 5 0 |0 0 2 |4 0 0
7 2 0 |0 0 0 |0 0 9
0 0 4 |0 0 0 |0 0 0
------+------+------
0 0 0 |1 0 7 |0 0 2
3 0 5 |0 0 0 |9 0 0
0 4 0 |0 0 0 |0 0 0
------+------+------
0 0 0 |0 8 0 |0 7 0
0 1 7 |0 0 0 |0 0 0
0 0 0 |0 3 6 |0 4 0
```

Important: zeros represent squares which do not have a value assigned yet. Having multiple zeroes in a row, column, or subgroup _does not_ make the puzzle invalid.

## How to know you're done

This exercise provides a set of high-level integration tests that will pass when you're done. You will very likely want to write additional unit tests to test-drive your classes.
