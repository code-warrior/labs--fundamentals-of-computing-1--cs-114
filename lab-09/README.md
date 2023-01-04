# Lab 9, CS 114, Fundamentals of Computing I

Remember **not** to work in this repository. Copy any files you need from this repo into another folder, then work from there.

---

## 1. Base Conversion

One algorithm for converting a base 10 number to another base `b` involves repeatedly dividing by `b`. Each time a division is performed, the remainder and quotient are saved. At each step, the dividend is the quotient from the preceding step; the divisor is always `b`. The algorithm stops when the quotient is `0`. The number in the new base is the sequence of remainders in reverse order (the last one computed goes first; the first one goes last).

In this exercise you will use this algorithm to write a program that converts a base 10 number to a 4-digit number in another base. The base 10 number and the new base (between 2 and 9) will be input to the program. The start of the program is in the file `BaseConvert.java`. Save this file to a different directory, then modify it to solve the problem presented in this lab.

---

## 2. Magic Squares

One interesting application of two-dimensional arrays is _magic squares_, which is a square matrix in which the sum of every row, every column, and both diagonals is the same. Magic squares have been studied for many years, and there are some particularly famous magic squares. In this exercise you will write code to determine whether a square is magic.

File `Square.java` contains the shell for a class that represents a square matrix. It contains headers for a constructor that gives the size of the square and methods to read values into the square, print the square, find the sum of a given row, find the sum of a given column, find the sum of the main (or other) diagonal, and determine whether the square is magic. The read method is given for you; you will need to write the others. Note that the read method takes a Scanner object as a parameter.

File `SquareTest.java` contains the shell for a program that reads input for squares from a file named `magicData` and tells whether each is a magic square. Following the comments, fill in the remaining code. Note that the main method reads the size of a square, then after constructing the square of that size, it calls the `readSquare` method to read the square in. The `readSquare` method _must_ be sent the `Scanner` object as a parameter.

You should find that the first, second, and third squares in the input are magic, and that the rest (fourth through seventh) are not. Note that the `-1` at the bottom tells the test program to stop reading.
