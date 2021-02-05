---
title: "Program to find Sum of digits of a Number using Recursion"
#date: 2021-02-05
draft: false
tags: ["recursion"]
---

## Program to find Sum of digits of a Number using Recursion

Below is a program to find sum of digits of a given number using recursion.

```c
#include<stdio.h>
#include<conio.h>

//declaring the recursive function
int sumOfDigit(int num);

void main()
{
    int num, sum;
    clrscr();
    printf("Enter a number:\t");
    scanf("%d", &num;);
    sum = sumOfDigit(num);
    printf("The sum of digits of %d is: %d", num, sum);
    getch();
}

int sumOfDigit(int num)
{
    int s, a;
    s = s + (num%10);
    a = num/10;
    if(a > 0)
    {
        sumOfDigit(a);
    }
    return s;
}
```
