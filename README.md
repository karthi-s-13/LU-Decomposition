# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
import numpy as np
### Step 2:
from scipy package import lu
### Step 3:
get input from the user
### Step 4:
print result
## Program:
(i) To find the L and U matrix
```
'''
Program to find L and U matrix using LU decomposition.
Developed by: KARTHIKEYAN S
RegisterNumber: 212224230116
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''
Program to solve a matrix using LU decomposition.
Developed by: KARTHIKEYAN S
RegisterNumber: 212224230116
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, piv = lu_factor(A)
x = lu_solve((lu, piv),B)
print(x)

```

## Output:
![Screenshot 2023-12-24 223621](https://github.com/gauthamkrishna7/LU-Decomposition/assets/141175025/e25eafca-eda8-4d9a-9b1c-b5599b970e49)
![Screenshot 2023-12-24 223653](https://github.com/gauthamkrishna7/LU-Decomposition/assets/141175025/3fc605ce-39cb-4765-a670-80740fc02a31)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

