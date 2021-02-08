---
title: "Swapping two Numbers using a Temporary Variable"
weight: 1
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Swapping two Numbers using a Temporary Variable

Below is a program to swap two numbers using temporary variable.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    int x = 10, y = 15, temp;
    temp = x;
    x = y;
    y = temp;
    printf("x = %d and y = %d", x, y);
    getch();
}
```

## Swapping tow Numbers without using a Temporary Variable

Below is a program to swap two numbers without using any temporary variable.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    int x = 10, y = 15;
    x = x + y - (y = x);
    printf("x = %d and y = %d",x,y);
    getch();
}
```

## Swapping two Numbers using Bitwise Operator

Below is a program to swap two numbers using bitwise operator.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    int x = 6, y = 4;
    x = x^y;
    y = x^y;
    x = x^y;
    printf("x = %d and y = %d", x, y);
    getch();
}
```

## Swapping two Numbers using Multiplication and Division

Below is a program to swap two numbers using multiplication and division.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    int x = 6, y = 4;
    x = x*y;
    y = x/y;
    x = x/y;
    printf("x = %d and y = %d", x, y);
    getch();
}
```
