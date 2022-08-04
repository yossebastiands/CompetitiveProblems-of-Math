Given a matrix of 𝑚×𝑛 and a folding direction, determine what the matrix will look like when folded in the given way.

Given four points on a piece of paper, assume the top left corner has a value of 1, and going in a clockwise direction, each corner increases in value by 1.
So its --> rectangle, with a number on each corner. Number 1 from top left, increase by 1 clockwise.

# Input Format

* The first line is the number of test cases (𝑡)
* The first line of each test case is the size of the matrix (𝑚 𝑛)
* The second line of each test case is the folding direction from point 𝑐 to 𝑑
* For the next 𝑚 lines, each line is the row of that matrix with 𝑛 values

# Constraints

* 1 ≤ 𝑐, 𝑑 ≤ 4 and 𝑐 ≠ 𝑑
* 1 ≤ 𝑚, 𝑛, 𝑡 ≤ 1,000,000
* 0 ≤ value inside the matrix (𝑣) ≤ 9
* When folded, if the value of 𝑣𝑖𝑗 that is folded over 𝑣𝑖’𝑗’ are not the same, we considered it asymmetrical (see Sample 3)
* If a side has the size of 1, we cannot fold perpendicularly to that side.

# Output Format

For each test case, print the number of the test case starting with 1 followed by the list of the resulting matrix of the folded paper. 
Use a hyphen symbol (-) for disappearing spaces. If the paper cannot be folded symmetrically, list “error.”


Sample Input 1

Input:
1
1 1
1 2
0

Sample Output 1
1
error

Sample Output 1 Explanation

The matrix has the size of 1×1, so it’s not foldable.

Sample Input 2

1
3 3
1 3
0 1 2
1 3 1
2 1 0

Sample Output 2

1
- -2
- 31
210

Sample Output 2 Explanation


If we fold it from corner 1 to corner 3, the numbers match the opposite numbers, so we can fold it symmetrically. 
The top left part has disappeared, so it is replaced with a hyphen symbol (-) in the output.

Sample Input 3

1
- -1 2
- 1 2
5 6

Sample Output 3

1
error

Sample Output 3 Explanation


We have a foldable matrix. 
However, when we fold from corner 1 to corner 2, the values inside the matrix are different (5 and 6), so we cannot fold it symmetrically.
