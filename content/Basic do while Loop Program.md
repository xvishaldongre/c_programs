---
title: "Basic do while Loop Program"
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Basic do while Loop Program

Every loop consists of three parts in sequence:

Do while loop is used when the actual code must be executed atleast once. For example: Incase of menu driven functions.

Below is a simple program on do while loop.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    /*
        always declare the variables before using them
    */
    int i = 10;     // declaration and initialization at the same time

    do // do contains the actual code and the updation
    {
        printf("i = %d\n",i);
        i = i-1;    // updation
    }
    // while loop doesn't contain any code but just the condition
    while(i > 0);

    printf("\n\The value of i after exiting the loop is %d\n\n", i);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
