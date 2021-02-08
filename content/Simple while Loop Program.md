---
title: "Simple while Loop Program"
weight: 1
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Simple while Loop Program

Every loop consists of three parts in sequence

Below is a simple program on while loop.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    /*
        always declare the variables before using them
    */
    int i = 0;  // declaration and initialization at the same time

    printf("\nPrinting numbers using while loop from 0 to 9\n\n");

    /*
        while i is less than 10
    */
    while(i<10)
    {
        printf("%d\n",i);

        /*
            Update i so the condition can be met eventually
            to terminate the loop
        */
        i++;    // same as i=i+1;
      }
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
