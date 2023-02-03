# CS232-Lab3

-----------------------------------------------------------------------------------

## Reading Material:
* [System calls in MIPS](https://courses.missouristate.edu/kenvollmar/mars/help/syscallhelp.html)
* [MIPS Cheat Sheet](https://inst.eecs.berkeley.edu/~cs61c/resources/MIPS_Green_Sheet.pdf)
* 

-----------------------------------------------------------------------------------

## Q1 (Capture the Flag!)
You are provided with 3 binary executables named as part_a, part_b, part_c. Use the objdump command to disassemble these executables, and read through them. 
* There is a function named `part_a(int)` which takes in an integer. You need to provide an integer such that the execution gives you a valid output. Any other input will result in termination.
* There is a function named `part_b(int, int, int)` which takes in three integers. You need to provide three integers such that the execution gives you a valid output. Any other input will result in termination.
* There is a function named `part_c(char*)` which takes in a string. You need to provide a string such that the execution gives you a valid output. Any other input will result in termination.

In README.md, provide clear insights on how you read through the assembly code, and how you discovered the implementation details. Finally, print the following string:
`{part 1’s output} + {part 2’s output} + {part 3’s output}`, where + denotes concatenation.

## Q2 (Find the inverse modulo m) - 20 points
Write an assembly program to find the inverse of a number a modulo m. Note that the inverse of `a` modulo `m` is the number `x` such that `ax = 1 (mod m)`. The program takes in input (format specified below) from a file named `input.txt`, and write it to a file named `output.txt`

### Input Format(`input.txt`):
a m

### Output Format(`output.txt`):
x 

### Constraints:
a, m are 64-bit positive integers.


## Q3 (Merge sort with a twist!)
Write an assembly program using MIPS ISA to sort an array of numbers using In-place merge sort, without  

## Q4 (The curious case of Matrix Multiplication)