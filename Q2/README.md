## Q2 (Find the inverse modulo m) - 10 points
Write an assembly program(`inverse.s`) using MIPS32 ISA to find the inverse of a number a modulo m. Note that the inverse of `a` modulo `m` is the number `x` such that `ax = 1 (mod m)`. 

* The program takes in input (format specified below) from a file named `input.txt`, and write it to a file named `output.txt`
* Make sure to include your approach with detailed explanation in the `report` file.
* If you have submitted a solution for the bonus part, clearly mention that in the `report` file. Not mentioning it will result in `0` marks for the bonus part.

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
* a, m are __32-bit__ positive integers.
* a, m are coprime.

## Constrains for Bonus part: (30 points)
* a, m are __32-bit__ positive integers.
* a, m are coprime