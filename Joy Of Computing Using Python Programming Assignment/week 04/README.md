#### Week 4: Programming Assignment 1
**Question** :

*Create a Python program that checks whether a given square matrix is diagonal. A diagonal matrix is a square matrix (same number of rows and columns) where all the entries outside the main diagonal are zero. The program should prompt the user to input the dimensions of the matrix and then input the matrix elements. The program should then determine whether the matrix is diagonal and print 1 if it is, otherwise print 0.*

##### source code :
```
def is_diagonal_matrix(matrix, r):
    for i in range(r):
        for j in range(r):
            if i != j and matrix[i][j] != 0:
                return 0
    return 1

r = int(input())

matrix = []
for _ in range(r):
    row = list(map(int, input().split()))
    matrix.append(row)

print(is_diagonal_matrix(matrix, r))
```

#### Week 4: Programming Assignment 2
**Question** :

*Create a Python program that adds the transpose of a given matrix by a scalar. The program should prompt the user to input the dimensions of the matrix, the elements of the matrix, and the scalar value. The program should then compute the transpose of the matrix, add it by the scalar, and print the resulting matrix.*

##### source code :
```
def add_transpose_by_scalar(matrix, r, c, s):
    result = [[matrix[j][i] + s for j in range(r)] for i in range(c)]
    return result

r = int(input())
c = int(input())

matrix = []
for _ in range(r):
    row = list(map(int, input().split()))
    matrix.append(row)

s = int(input())

result_matrix = add_transpose_by_scalar(matrix, r, c, s)

for row in result_matrix:
    print(" ".join(map(str, row)))
```
#### Week 4: Programming Assignment 3
**Question** :

*Create a Python program that checks whether a given square matrix is symmetric. A matrix is symmetric if its transpose is equal to the matrix itself. The program should prompt the user to input the dimensions of the matrix and then input the matrix elements. The program should then determine whether the matrix is symmetric and print 1 if it is, otherwise print 0.*

##### source code :
```
def is_symmetric(matrix, r):
    for i in range(r):
        for j in range(r):
            if matrix[i][j] != matrix[j][i]:
                return 0
    return 1

r = int(input())

matrix = []
for _ in range(r):
    row = list(map(int, input().split()))
    matrix.append(row)

print(is_symmetric(matrix, r))
```
