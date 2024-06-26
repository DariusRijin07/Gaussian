# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. At first, we have imported the necessary libraries we will use in our program.

2. Read Number of Unknowns: n

3. Read Augmented Matrix (A) of n by n+

4. Transform Augmented Matrix (A) to Upper Trainagular Matrix by Row Operations.

5. After that, we applied the Gaussian elimination method.

6. After that, we apply the back substitution method to obtain the desired output.

7. Display Result.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by:  Darius Rijin I
RegisterNumber:212223230037
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
![gaussian elimination]()
![3](https://github.com/DariusRijin07/Gaussian/assets/138849120/15949c14-5bb8-4336-8e52-879d9ccff5c7)
![4](https://github.com/DariusRijin07/Gaussian/assets/138849120/ad13986c-9fc5-4049-8add-95ec5f1132af)


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

