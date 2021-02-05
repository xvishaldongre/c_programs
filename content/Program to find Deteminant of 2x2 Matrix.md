---
title: "Program to find Deteminant of 2x2 Matrix"
#date: 2021-02-05
draft: false
tags: ["array"]
---

## Program to find Deteminant of 2x2 Matrix

Below is a program to find the determinant of a 2x2 matrix.

Please note that, when we say a 2x2 matrix, we mean an array of 2x2.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    int a[2][2], i, j;
    long determinant;

    printf("\n\nEnter the 4 elements of the array\n");
    for(i = 0; i < 2; i++)
    for(j = 0; j < 2; j++)
    scanf("%d", &a[i][j]);

    printf("\n\nThe entered matrix is: \n\n");
    for(i = 0; i < 2; i++)
    {
        for(j = 0; j < 2; j++)
        {
            printf("%d\t", a[i][j]);   // to print the complete row
        }
        printf("\n"); // to move to the next row
    }

    // finding the determinant of a 2x2 matrix
    determinant = a[0][0]*a[1][1] - a[1][0]*a[0][1];
    printf("\n\nDterminant of 2x2 matrix is : %d - %d =  %d", a[0][0]*a[1][1], a[1][0]*a[0][1], determinant);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
