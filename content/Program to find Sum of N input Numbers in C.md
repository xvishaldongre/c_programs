---
title: "Program to find Sum of N input Numbers in C"
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Program to find Sum of N input Numbers in C

Below is a program on sum of n numbers.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n,sum=0,c,value;

    printf("\n\nEnter the number of integers you want to add:  ");
    scanf("%d", &n);

    printf("Enter %d integers\n\n",n);
    for(c = 1; c <= n; c++)
    {
        scanf("%d", &value);
        /*
            need to initialise sum before using otherwise
            garbage value will get printed
        */
        sum += value;
    }

    printf("\n\n\nsum of entered numbers  = %d", sum);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
