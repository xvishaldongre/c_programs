---
title: "Basic program to show use of nested for Loops"
weight: 1
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Basic program to show use of nested for Loops

Nested loops are usually used to print a pattern in C. They are also used to print out the matrix using a 2 dimensional array and a lot of other patterns like pyramid of numbers etc.

Using a loop inside another loop is called nested loop.

Below is a simple program on nested loops.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    printf("\n\nNested loops are usually used to print a pattern in c. \n\n");
    printf("\n\nThey are also used to print out the matrix using a 2 dimensional array. \n\n");

    int i,j,k;
    printf("\n\nOutput of the nested loop is :\n\n");
    for(i = 0; i < 5; i++)
    {
        printf("\t\t\t\t");
        for(j = 0; j < 5; j++)
        printf("* ");

        printf("\n");
    }
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
