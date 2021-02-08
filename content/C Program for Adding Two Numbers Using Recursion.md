---
title: "C Program for Adding Two Numbers Using Recursion"
weight: 1
#date: 2021-02-05
draft: false
tags: ["recursion"]
---

## C Program for Adding Two Numbers Using Recursion

Below is a program on adding two numbers using recursion.

```c
#include<stdio.h>

int y;

/*
    Function to add two numbers and
    return the result
*/
int add(int m, int n)
{
    if(n == 0)
        return m;

    /*
        Recursion: adding 1, n times and
        then at the end adding m to it
    */
    y = add(m, n-1) + 1;
    return y;   // return the result
}

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int a, b, r;
    printf("Enter the two numbers:\n");
    scanf("%d%d", &a, &b);
    r = add(a, b);     // function call
    printf("\n\nSum of two numbers is: %d\n\n", r);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
