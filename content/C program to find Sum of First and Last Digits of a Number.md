---
title: "C program to find Sum of First and Last Digits of a Number"
weight: 1
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C program to find Sum of First and Last Digits of a Number

Note: % or the mod operator is used to find the remainder of division operation.

Below is a program to find sum of first and last digits of the user input number.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int input, firstNumber, lastNumber;

    printf("Enter a number: ");
    scanf("%d", &input);

    /*
        gives remainder when the input value is divided by 10
        i.e. the digit at units place
    */
    lastNumber = input%10;

    firstNumber = input;

    while(firstNumber >= 10)
    {
        firstNumber /= 10;  // same as firstNumber = firstNumber/10
    }

    printf("\n\n\nAddition of first and last number is: %d + %d = %d\n", firstNumber, lastNumber, firstNumber+lastNumber);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
