---
title: "C program to show basic Arithmetic Operations and role of Typecasting"
weight: 1
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C program to show basic Arithmetic Operations and role of Typecasting

Here we have 2 simple programs to showcase various basic arithmetic operations and how typecasting is handled by C language with and without explicitly using Typecasting in our program.

## Arithmetic Operations without Typecasting

Below is a program to perform basic arithmetic operations without typecasting.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int a, b, add, subtract, multiply;
    float divide;

    printf("Enter two integers: \n");
    scanf("%d%d", &a, &b);

    add = a+b;
    subtract = a-b;
    multiply = a*b;
    divide = a/b;

    printf("\nAddition of the numbers = %d\n", add);
    printf("Subtraction of 2nd number from 1st = %d\n", subtract);
    printf("Multiplication of the numbers = %d\n", multiply);
    printf("Dividing 1st number from 2nd = %f\n", divide);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Arithmetic Operations with Typecasting

C Language do handle typecasting implicitly, still user can handle it in their programs too.

Below is a simple program to perform basic arithmetic operations with typecasting.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    int a, b, add, subtract, multiply, remainder;
    float divide;

    printf("Enter two integers: \n");
    scanf("%d%d", &a, &b);

    add = a+b;
    subtract = a-b;
    multiply = a*b;
    divide = a/(float)b;
    remainder = a%b;

    printf("\n\nAddition of the numbers = %d\n", add);
    printf("\nSubtraction of 2nd number from 1st = %d\n", subtract);
    printf("\nMultiplication of the numbers = %d\n", multiply);
    printf("\nDividing 1st number from 2nd = %f\n", divide);
    printf("\nRemainder on Dividing 1st number by 2nd is %d\n", remainder);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
