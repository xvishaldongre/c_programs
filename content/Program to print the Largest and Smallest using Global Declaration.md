---
title: "Program to print the Largest and Smallest using Global Declaration"
weight: 1
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Program to print the Largest and Smallest using Global Declaration

Some important points about Global variable declaration are:

%0nd is used to represent numbers in n digit format with leading 0's.

Below is a program to find largest and smallest value using global declaration.

```c
#include<stdio.h>

int a,b;
int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    printf("\n\nEnter the two values to find the greatest and smallest number: \n");
    scanf("%d%d", &a, &b);

    if(a == b)
        printf("Both are equal\n");

    else if(a < b)
    {
        printf("\n\nThe largest number is %03d\n", b);
        printf("\nThe smallest number is %03d\n", a);
        printf("\nThe largest number is %03d\n", b);
    }
    else    //Only possibility remaining
    {
        printf("The largest number is %03d\n", a);
        printf("The smallest number is %03d\n", b);
    }
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
