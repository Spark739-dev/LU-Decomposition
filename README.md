# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Step1: Import numpy and scipy.linalg ,in linalg you can input lu and in second program can import lu_factor and lu_solve from python library as same as in second program.

2. Step2:Get the input from user as the form of nested list to compute numpy array as same as in second program. 
3.Step 3: Use  inputted array to compute lu decomposition and solve them by using corresponding inbulit modules of numpy and scipy.
4. Step4:Print the corresponding varaiable to declare the output as results.

## Program:

```
'''Program to find L and U matrix using LU decomposition.
Developed by: veshwanth
RegisterNumber: 24010033
'''
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)

```

use lu decomposition to solve a matrix


```
'''Program to solve a matrix using LU decomposition.
Developed by: veshwanth
RegisterNumber: 24010033
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
b=np.array(eval(input()))
x=lu_factor(matrix)
solution=lu_solve(x,b)
print(solution)

```

## Output:
![lu decomposition](output.png)
![lu decomposition to solve a matrix](output2.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

