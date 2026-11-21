# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required libraries, NumPy and SciPy, for performing LU decomposition and solving linear equations.

2.Get the square matrix A as input and perform LU decomposition using lu(A). Store the permutation, lower triangular, and upper triangular matrices in P, L, and U, respectively, and display L and U.

3.Get the coefficient matrix A and the constant vector b as input. Perform LU factorization using lu_factor(A) and solve the system of linear equations using lu_solve((lu, piv), b). Store the solution in X.

4.Display the solution X and Stop the program.
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: CHANDRU V
RegisterNumber: 212224230043
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: CHANDRU V
RegisterNumber: 212224230043
'''
# To print X matrix (solution to the equations)

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
```

## Output:

<img width="1195" height="507" alt="image" src="https://github.com/user-attachments/assets/fefd4f84-58f5-428b-982e-f2ee47676bdc" />


<img width="892" height="302" alt="image" src="https://github.com/user-attachments/assets/d88e9428-b081-4780-95fc-73a2a6091cc4" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

