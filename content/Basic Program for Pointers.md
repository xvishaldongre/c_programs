---
title: "Basic Program for Pointers"
weight: 1
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Basic Program for Pointers

Few important points to remember:

Below is a simple program on pointer.

int \*p; is a pointer variable declaration where p is a pointer to an int variable i.e. it stores the location of an integer.

%x is a format specifier to print hexadecimal value. It is usually used to print the location.

```c
#include <stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int var = 24;   // actual variable declaration
    int *p;

    p = &var;   // storing address of int variable var in pointer p

    printf("\n\nAddress of var variable is: %x \n\n", &var);

    // address stored in pointer variable
    printf("\n\nAddress stored in pointer variable p is: %x", p);

    // access the value using the pointer variable
    printf("\n\nValue of var variable or the value stored at address p is   %d ", *p);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
