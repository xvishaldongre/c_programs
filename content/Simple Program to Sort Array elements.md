---
title: "Simple Program to Sort Array elements"
#date: 2021-02-05
draft: false
tags: ["array"]
---

## Simple Program to Sort Array elements

Below is a program to sort array elements in an array.

```c
#include<stdio.h>
#include<conio.h>

void sorting(int *x, int y);

void main()
{
    int a[20], i, c, n;
    clrscr();
    printf("Enter number of elements you want to sort: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    scanf("%d", &a[i]);

    sorting(a, n);

    for(i = 0; i <n; i++)
    printf("%d\t", a[i]);

    getch();
}

void sorting(int *x, int y)
{
    int i, j, temp;
    for(i = 1; i <= y-1; i++)
    {
        for(j = 0; j < y-i; j++)
        {
            if(*(x+j) > *(x+j+1))
            {
                temp = *(x+j);
                *(x+j) = *(x+j+1);
                *(x+j+1) = temp;
            }
        }
    }
}
```
