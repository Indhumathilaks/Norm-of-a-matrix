# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No: 212224220037
# Developed By: INDHUMATHI L
# 1-Norm of a Matrix

import ast
A=ast.literal_eval(input())
n=len(A)
m=len(A[0])
one_norm=max(sum(abs(A[i][j]) for i in range(n)) for j in range(m))
print(f"{one_norm:.2f}")


# 2-Norm of a Matrix

import numpy as np
mat=np.array(eval(input()))
ans=np.linalg.norm(mat,2)
Norm_of_matrix='{:.2f}'.format(ans)
print(Norm_of_matrix)


# Infinity Norm of a Matrix

import numpy as np
mat=np.array(eval(input()))
ans=np.linalg.norm(mat,np.inf)
Norm_of_matrix="{:.2f}".format(ans)
print(Norm_of_matrix)



```
## Output:
### 1-Norm of a Matrix
<img width="1161" height="902" alt="image" src="https://github.com/user-attachments/assets/14b50ebc-b089-45cd-af14-406fc8fad598" />


### 2-Norm of a Matrix
<img width="1012" height="934" alt="image" src="https://github.com/user-attachments/assets/34f589bb-ce0b-4512-bab1-1697ce2011bc" />


### Infinity Norm of a Matrix
<img width="1112" height="889" alt="image" src="https://github.com/user-attachments/assets/715c6a6c-3c0c-4418-9b85-6f59b19a8c9e" />


## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
