# CS232-Lab3

VIVA will be conducted for this Lab.

-----------------------------------------------------------------------------------

## Reading Material:
* [System calls in MIPS](https://courses.missouristate.edu/kenvollmar/mars/help/syscallhelp.html)
* [MIPS Cheat Sheet](https://inst.eecs.berkeley.edu/~cs61c/resources/MIPS_Green_Sheet.pdf)
* 
-----------------------------------------------------------------------------------

## Common Grading Schema:
* If the program doesn't run (or) aborts => `0` marks

## Q1 (Capture the Flag!) - 50 points
You are provided with 3 binary executables named as part_a, part_b, part_c. Use the objdump command to disassemble these executables, and understand them and obtain a valid output from them. 
* For part_a, the program takes in only a integer input \[definition: part_a(int)\] . A valid input results in a valid output while any other input terminates the program.
* For part_b, the program takes in 3 integer inputs \[definition: part_b(int,int,int)\]. Given a valid triplet you obtain a valid output, while every other branch terminates.
* For part_c, the program takes in a string input \[definition: part_c(char*)\]. A specific null-terminated string results in a valid output, in all other cases the program terminates

In README.md, provide clear insights on how you read through the assembly code, and how you discovered the implementation details. Finally, print the following string into your README:
`{part 1’s output} + {part 2’s output} + {part 3’s output}`, where + denotes concatenation.

### Grading Scheme:
* Correct Flag, no explanation => `0` marks
* Incorrect flag, but reasonable explanation => `20` marks
* Correct Flag, correct explanation => `50` marks

## Q2 (Find the inverse modulo m) - 20 points
Write an assembly program to find the inverse of a number a modulo m. Note that the inverse of `a` modulo `m` is the number `x` such that `ax = 1 (mod m)`. 

The program takes in input (format specified below) from a file named `input.txt`, and write it to a file named `output.txt`

### Input Format(`input.txt`):
```
a 
m
```

### Output Format(`output.txt`):
```
x 
```

### Constraints:
a, m are 64-bit positive integers.

### Grading Scheme:
* Executes, but incorrect result: `0` marks
* Executes, correct results for a, m being 32-bit integers => `10` marks
* Executes, correct results for all a, m => `20` marks

## Q3 (Merge sort with a twist!) - 50 points
Write an assembly program using MIPS ISA to sort an array of numbers using In-place merge sort(merge sort without using extra additional space). The time complexity should be `O(nlogn)`, while the additional space complexity should be `O(1)`.

The program takes in input (format specified below) from a file named `input.txt`, and write it to a file named `output.txt`

### Input Format(`input.txt`):
```
N
a1
a2
...
aN
```

### Output Format(`output.txt`):
```
b1
b2
...
bN
```

where `(b1, b2, ..., bn)` denotes the sorted version of `(a1, a2, ..., an)`

### Constraints:
* `N <= 10000`
* `a_i <= 10000` for all `i = 1, 2, ..., N`

### Grading Scheme:
* Executes, but incorrect result => `0` marks
* Correct result, time complexity is worse than `O(n^2)`:
  * If additional space complexity is `O(1)` => `30` marks
  * Else => `20` marks
* Correct result, time complexity is `O(nlogn)`:
  * If additional space complexity is `O(1)` => `50` marks
  * Else => `30` marks

## Q4 (The curious case of Matrix Multiplication) - 80 points
