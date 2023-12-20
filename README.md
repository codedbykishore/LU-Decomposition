# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
1. Import lu from scipy.linalg package
2. Import numpy module
3. Create the matrix
4. Use lu to find the L and U matrix
5. Print the L and U matrix

(ii)
1. Import lu_factor and lu_solve from scipy.linalg package
2. Import numpy module
3. Create the matrix
4. Take a constant as input
5. Use lu_factor to find the factor
6. Use lu_solve to find the solution
7. Print the solution
## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: KISHORE B
RegisterNumber: 23013723
'''
from scipy.linalg import lu
import numpy as np
A=eval(input())
X=np.array(A)
P,L,U=lu(X)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''Program to solve a matrix using LU decomposition.
Developed by: KISHORE B
RegisterNumber: 23013723
'''
from scipy.linalg import lu_factor,lu_solve
# To print X matrix (solution to the equations)
import numpy as np
arr=eval(input())
constant=eval(input())
A=np.array(arr)
B=np.array(constant)
result=lu_factor(A)
solution=lu_solve(result,B)
print(solution)
```

## Output:
![Screenshot from 2023-12-20 20-39-33](https://github.com/codedbykishore/LU-Decomposition/assets/147139122/3d767783-23ca-4125-9bc1-cdb298e72c56)
<br>
![Screenshot from 2023-12-20 20-41-53](https://github.com/codedbykishore/LU-Decomposition/assets/147139122/4b84f78f-a090-4947-b90b-b6172c09ffbd)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

