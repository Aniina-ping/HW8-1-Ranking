# HW8-1-Ranking
You are given a struct of `Node` and a Table that stores `Node*`. Your task is to complete the following 3 operations in `rank.c` and using makefile to test your code.

There are 3 types of operations:
'A': Insert
- followed by `score` and `name` of inserted node 
- add Node* with (score, name) into Table

'B': Delete
- followed by `name`
- delete the Node* with `name` in the Table

'C': Top x
- followed by `x`
- return int array contains the indices of top x Nodes in Table

The rank of Node* is defined below:
- The higher score => the higher rank
- If same score => ranking by their names in lexicological order

Input:
First line contains 1 number t, t is the number of test cases.
There’s 1 operation on the each of following t lines.

- Constraint:
    - 1 ≤ t ≤ 100
    - The number of elements in Table will not exceed 100 during the process
    - 1 ≤ The length of all names ≤ 100, all names are distinct and start with an uppercase letter 
    - 0 ≤ score ≤ 100
    - It guaranteed that if there are no elements in the Table, the delete operation will not be executed 

Output:
- Print the top x names in the Table for each TOP x operation.
- Each output is followed by a newline
- The format will be like this:
```
Top 2:
33 Kevin
10 John
```
How to test your code?
1. Please `make clean` first and execute `make all` to generate a executable file.
2. Run `make runtest`. If your get the `Test passed` message in four testcases, Congratulations!! 
Otherwise, please fixed the BUGS...

Note: In homework8-1, the file that you should submit are `main.c`, `rank.h`, `rank.c`, and `makefile`.
