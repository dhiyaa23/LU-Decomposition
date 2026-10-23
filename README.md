# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the NumPy module to use the built-in functions for calculation
2. Prepare the lists from the given matrix and assign in np.array()
3. Use scipy.linalg.lu_factor() to compute LU factors and pivot indices for efficient solving.
4. Use scipy.linalg.lu_solve() to find the solution vector x.
5. End program
## Program:
(i) To find the L and U matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
/*
Program to find the L and U matrix.
Developed by: Dhiyaashni.D.K
RegisterNumber: 26007521
*/
```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
/*
Program to find the LU Decomposition of a matrix.
Developed by: Dhiyaashni.D.K
RegisterNumber: 26007521
*/
```

## Output:)
<img width="1315" height="867" alt="math lu 1" src="https://github.com/user-attachments/assets/9860cc01-3d25-478d-861e-726619723a24" />
<img width="1312" height="827" alt="math lu 2" src="https://github.com/user-attachments/assets/377ace24-9dc7-49e1-a08d-ee693b341f55" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

