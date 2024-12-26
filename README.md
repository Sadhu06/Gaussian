# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Input the Number of unknowns:Read the integer n.
2. Initialize the augmented matrix.
3. Fill the Augmented Matrix and check for zero on the diagonal.
4. Compute row elimination and check for singular matrix.
5. Use back substitution and output the solutions.
6. End the program.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Sadhana S
RegisterNumber: 24001394
import numpy as np
n=int(input())
matrix=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        matrix[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=matrix[j][i]/matrix[i][i]
        for k in range(n+1):
            matrix[j][k]=matrix[j][k]-ratio*matrix[i][k]
#Back substitution
x[n-1]=matrix[n-1][n]/matrix[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=matrix[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-matrix[i][j]*x[j]
    x[i]=x[i]/matrix[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,x[i]),end=" ")

*/
```

## Output:
![Screenshot from 2024-12-26 11-45-48](https://github.com/user-attachments/assets/541f92c4-f7b9-46c8-80a6-4d0e9648945e)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

