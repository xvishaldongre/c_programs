---
title: "C Program to find LCM of two Numbers using Recursion"
#date: 2021-02-05
draft: false
tags: ["recursion"]
---

## C Program to find LCM of two Numbers using Recursion

LCM: Least Common Multiple of two numbers is the number that is a common multiple of the both the numbers.

Below is a program to find LCM of two numbers using recursion.

```c
#include<stdio.h>

int find_lcm(int, int);   // function prototype declaration

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int a, b, lcm;
    printf("\n\nEnter 2 integers to find LCM of:\n");
    scanf("%d%d", &a, &b);
    lcm = find_lcm(a,b);    // function call
    printf("\n\n LCM of %d and %d is: %d\n\n", a, b, lcm);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

int find_lcm(int a, int b)  // function definition
{
    /*
        static variable is initialized only once
        for each function call
    */
    static int temp = 1;
    if(temp%a == 0 && temp%b == 0)
    {
        return temp;
    }
    else
    {
        temp++;
        find_lcm(a,b);
        return temp;
    }
}
```
