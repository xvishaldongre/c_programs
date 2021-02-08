---
title: "Simple Program to remove Duplicate Element in an Array"
weight: 1
#date: 2021-02-05
draft: false
tags: ["array"]
---

## Simple Program to remove Duplicate Element in an Array

Below is a program to find and remove any duplicate element present in the specified array.

```c
#include<stdio.h>
#include<conio.h>
void main()
{
    int a[20], i, j, k, n;
    clrscr();

    printf("\nEnter array size: ");
    scanf("%d", &n;);

    printf("\nEnter %d array element: ", n);
    for(i = 0; i < n; i++)
    {
        scanf("%d", &a;[i]);
    }

    printf("\nOriginal array is: ");
    for(i = 0; i < n; i++)
    {
        printf(" %d", a[i]);
    }

    printf("\nNew array is: ");
    for(i = 0; i < n; i++)
    {
        for(j = i+1; j < n; )
        {
            if(a[j] == a[i])
            {
                for(k = j; k < n; k++)
                {
                    a[k] = a[k+1];
                }
                n--;
            }
            else
            {
                j++;
            }
        }
    }

    for(i = 0; i < n; i++)
    {
        printf("%d ", a[i]);
    }
    getch();
}
```
