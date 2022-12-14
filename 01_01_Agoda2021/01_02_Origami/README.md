Given a matrix of πΓπ and a folding direction, determine what the matrix will look like when folded in the given way.

Given four points on a piece of paper, assume the top left corner has a value of 1, and going in a clockwise direction, each corner increases in value by 1.
So its --> rectangle, with a number on each corner. Number 1 from top left, increase by 1 clockwise.

# Input Format

* The first line is the number of test cases (π‘)
* The first line of each test case is the size of the matrix (π π)
* The second line of each test case is the folding direction from point π to π
* For the next π lines, each line is the row of that matrix with π values

# Constraints

* 1 β€ π, π β€ 4 and π β  π
* 1 β€ π, π, π‘ β€ 1,000,000
* 0 β€ value inside the matrix (π£) β€ 9
* When folded, if the value of π£ππ that is folded over π£πβπβ are not the same, we considered it asymmetrical (see Sample 3)
* If a side has the size of 1, we cannot fold perpendicularly to that side.

# Output Format

For each test case, print the number of the test case starting with 1 followed by the list of the resulting matrix of the folded paper. 
Use a hyphen symbol (-) for disappearing spaces. If the paper cannot be folded symmetrically, list βerror.β


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

The matrix has the size of 1Γ1, so itβs not foldable.

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
