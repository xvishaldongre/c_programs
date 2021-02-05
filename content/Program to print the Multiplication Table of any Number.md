---
title: "Program to print the Multiplication Table of any Number"
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Program to print the Multiplication Table of any Number

Below is a program to print the multiplication table of any user input number.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n,i;

    printf("Enter an integer you need to print the table of: ");
    scanf("%d", &n);
    printf("\n\n\n");

    for(i = 1; i <= 10; i++)
    {
        printf("\n\t\t\t%d * %d   =   %d \n", n, i, n*i);
    }

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
