---
title: "Program to take input of various datatypes in C"
weight: 1
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Program to take input of various datatypes in C

Below is a program to explain how to take input from user for different datatypes available in C language. The different datatypes are int(integer values), float(decimal values) and char(character values).

printf() is used to display text onto the screen

& is used to assign the input value to the variable and store it at that particular location.

scanf() is uded to take input from the user using format specifier discussed in upcoming tutorials

%d and %i, both are used to take numbers as input from the user.

%f is the format specifier to take float as input from the user

%s is the format specifier to take character as input from the user

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    int num1, num2;
    float fraction;
    char character;

    printf("Enter two numbers number\n");

    // Taking integer as input from user
    scanf("%d%i", &num1, &num2);
    printf("\n\nThe two numbers You have entered are %d and %i\n\n", num1, num2);

    // Taking float or fraction as input from the user
    printf("\n\nEnter a Decimal number\n");
    scanf("%f", &fraction);
    printf("\n\nThe float or fraction that you have entered is %f", fraction);

    // Taking Character as input from the user
    printf("\n\nEnter a Character\n");
    scanf("%c",&character);
    printf("\n\nThe character that you have entered is %c", character);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");

    return 0;
}
```
