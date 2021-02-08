---
title: "Basic C Program for Pointer to a Pointer"
weight: 1
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Basic C Program for Pointer to a Pointer

A pointer variable stores the address of a value. Similarly, a pointer to a pointer stores the address of the pointer variable. Pointer to a pointer is executed making use of \*\*.

Below is a program on pointer to a pointer.

int var; is a integer variable which stores value.

int \*ptr; is a pointer variable which stores the address of an integer variable.

int \*\*pptr; is a pointer to a pointer variable which stores the address of a pointer variable.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int var;
    int *ptr;
    int **pptr;

    var = 50;

    // take the address of the variable var
    ptr = &var;

    // taking the address of ptr using address of operator-&
    pptr = &ptr;

    // take the value using the pptr
    printf("\n\nValue of var = %d\n\n", var);

    printf("\n\nValue available at *ptr = %d\n\n", *ptr);

    printf("\n\nValue available at **pptr = %d\n\n", **pptr);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
