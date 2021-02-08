---
title: "Program to find Factors of a Number"
weight: 1
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Program to find Factors of a Number

Below is a program to find factors of a number.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int  num, i;
    printf("Enter the number to find the factors of :  ");
    scanf("%d",&num);
    printf("\n\n\nFactors of %d are \n\n", num);

    for(i = 1; i <= num/2; i++)
    {
        if(num%i == 0)
            printf("\t\t\t%d\n", i);
    }

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
