# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix
1. The user is prompted to enter a matrix in the form of a nested list. 
2. The lu function performs LU decomposition with partial pivoting.
𝑃 Permutation matrix (to reorder rows for numerical stability).
𝐿 Lower triangular matrix (with ones on the diagonal).
𝑈 Upper triangular matrix.
3. The L and U matrices are printed to the console.
4. End of the program
(ii) To find the LU Decomposition of a matrix
1.  A square matrix representing coefficients of the linear equations. A column vector representing the right-hand side of the equations.
2.  LU Factorization: lu_factor(A) performs an LU decomposition with partial pivoting, returning:
    piv: A pivoting information array.
3.Solving Ax=b. lu_solve((lu, piv), b) solves the equation efficiently using the LU decomposition.
4.End of the porgram
## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: 212224230116
RegisterNumber: KARTHIKEYAN S
*/
```
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: 212224230116
RegisterNumber: KARTHIKEYAN S
*/
```
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
``` 

## Output:
![Screenshot 2024-12-04 160034](https://github.com/user-attachments/assets/5714ed88-867e-4140-ad55-e7d0e7e4f93a)
![Screenshot 2024-12-04 160613](https://github.com/user-attachments/assets/9eac93d3-d86c-4e4d-90ce-bd9bbca844fc)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

