---
title: "C program to Check for a Perfect Square"
weight: 1
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C program to Check for a Perfect Square

Below is a program to check whether the user input number is a perfect square or not.

```c
#include<stdio.h>
int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    // variable declaration
    int i, number;

    // take user input
    printf("Enter a number: ");
    scanf("%d", &number);

    // loop to check number is perfect square or not
    for(i = 0; i <= number; i++)
    {
        if(number == i*i)
        {
            printf("\n\n\n\t\t\t%d is a perfect square\n\n\n", number);

            printf("\n\n\t\t\tCoding is Fun !\n\n\n");
            return 0;   // same as using break in this case to end the program
        }
    }
    printf("\n\n\n\t\t\t%d is not a perfect square\n", number);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
