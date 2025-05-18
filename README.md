# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
```
Step 1: Input the matrix A from the user.
Step 2: Perform LU decomposition on A to obtain P, L, U such that PA = LU.
Step 3: Extract the lower triangular matrix L and upper triangular matrix U.
Step 4: Print the matrices L and U.

(ii)
Step 1: Input the matrix A and the vector b from the user.
Step 2: Compute the LU factorization of A using lu_factor to get lu and piv.
Step 3: Solve the system AX = b by applying lu_solve with the LU factors and pivots.
Step 4: Print the solution vector X.  
```
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: K.Dilli babu
RegisterNumber: 212224110015
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: K.Dilli Babu
RegisterNumber: 212224110015
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
# 1 st:
![Screenshot 2025-04-26 143012](https://github.com/user-attachments/assets/a8bdf012-9094-406a-944b-0d25978df725)
# 2 nd:
![Screenshot 2025-04-26 143022](https://github.com/user-attachments/assets/5650ab9e-8ce3-4ffd-9bcd-4d688c120e9c)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

