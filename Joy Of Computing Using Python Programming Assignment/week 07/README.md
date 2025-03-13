### Week 7: Programming Assignment 1
**Question**
***Magic Square***

A magic square of order n is a square arrangement of n2 numbers, typically distinct integers, where the sum of the n numbers in each row, each column, and both main diagonals is the same constant. It consists of the integers from 1 to .

The constant sum of each row, column, and diagonal in a magic square is known as the magic constant or magic sum, M. For a normal magic square, this constant depends solely on n and is given by the formula

**Source Code**

```
def is_magic_square(matrix, n):
    magic_sum = n * (n**2 + 1) // 2

    for row in matrix:
        if sum(row) != magic_sum:
            return "Not a Magic Matrix"

    for col in range(n):
        if sum(matrix[row][col] for row in range(n)) != magic_sum:
            return "Not a Magic Matrix"

    if sum(matrix[i][i] for i in range(n)) != magic_sum:
        return "Not a Magic Matrix"

    if sum(matrix[i][n - 1 - i] for i in range(n)) != magic_sum:
        return "Not a Magic Matrix"

    return "Magic Matrix"

n = int(input())
matrix = [list(map(int, input().split())) for _ in range(n)]

print(is_magic_square(matrix, n))
```
### Week 7: Programming Assignment 2
**Question**
***Median of Matrix***

You are given a row-wise sorted matrix of size n×m, where both the number of rows and the number of columns are always odd. Your task is to find the median of the matrix.

The median is the middle number in a sorted list of numbers. In case the list has an even number of elements, the median is the leftmost of the two middle elements.

The matrix is sorted row-wise, but the entire matrix is not necessarily sorted.

You need to find the median from the matrix when all the elements are sorted in ascending order.

**Source Code**
```
def find_median(matrix, n, m):
    elements = [num for row in matrix for num in row]
    elements.sort()
    median = elements[(n * m) // 2]
    return median

n, m = map(int, input().split())
matrix = [list(map(int, input().split())) for _ in range(n)]

print(find_median(matrix, n, m))
```
### Week 7: Programming Assignment 3
**Question**
***Rotate a Rectangular Image by 90 Degrees Clockwise***

You are given an image represented by an m x n matrix. Your task is to rotate the image by 90 degrees in the clockwise direction. After rotation, the dimensions of the result matrix will be n x m, as the number of rows and columns will be swapped.

**Source Code**
```
def rotate_matrix_clockwise(matrix, m, n):
    rotated_matrix = [[0] * m for _ in range(n)]

    for i in range(m):
        for j in range(n):
            rotated_matrix[j][m - 1 - i] = matrix[i][j]

    for row in rotated_matrix:
        print(*row)

m, n = map(int, input().split())
matrix = [list(map(int, input().split())) for _ in range(m)]

rotate_matrix_clockwise(matrix, m, n)

```
