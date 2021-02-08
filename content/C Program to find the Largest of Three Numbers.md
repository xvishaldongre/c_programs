---
title: "C Program to find the Largest of Three Numbers"
weight: 1
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C Program to find the Largest of Three Numbers

Below is a program to find the largest amongst the three user input numbers.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    float a, b, c;

    printf("Enter 3 numbers:\n\n");
    scanf("%f%f%f", &a, &b, &c);

    if(a >= b && a >= c)
    {
        /*
            %.3f prints the floating number
            upto 3 decimal places
        */
        printf("\n\nLargest number = %.3f ", a);
    }
    else if(b >= a && b >= c)
    {
        printf("\n\nLargest number is = %.3f", b);
    }
    else
    {
        printf("\n\nLargest number is = %.3f", c);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
