---
title: "Program to find exponential without using pow() method"
weight: 1
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Program to find exponential without using pow() method

Below is a program to find exponential without using pow() method.

long long int is of double the size of long int.

%lld is the format specifier for long long int.

```c
#include<stdio.h>
int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    int n, exp, exp1;
    long long int value = 1;

    printf("Enter the number and its exponential:\n\n");
    scanf("%d%d",&n, &exp);

    exp1 = exp;   // storing original value for future use

    // same as while((--exp)!=-1)
    while(exp-- > 0)
    {
        value *= n; // multiply n to itself exp times
    }

    printf("\n\n %d^%d = %lld\n\n", n, exp1, value);
    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
