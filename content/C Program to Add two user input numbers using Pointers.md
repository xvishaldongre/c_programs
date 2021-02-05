---
title: "C Program to Add two user input numbers using Pointers"
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C Program to Add two user input numbers using Pointers

Few important points to remember:

Below is a program adding two numbers using pointers.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int first, second, *p , *q, sum;
    printf("Enter two integers to add using pointers:\n");
    scanf("%d%d", &first, &second);
    p = &first;
    q = &second;
    sum = *p + *q;
    printf("\n\nThe sum of the entered numbers is: %d", sum);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
