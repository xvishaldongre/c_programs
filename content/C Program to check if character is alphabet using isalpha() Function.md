---
title: "C Program to check if character is alphabet using isalpha() Function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["CTYPE.H"]
---

## C Program to check if character is alphabet using isalpha() Function

In this program we will check if a character is an alphabet or not. We will be using a system defined function isalpha() defined under the ctype.h library.

This can also be done using if-else blocks condition using the range of the ASCII values of the alphabets. This method is used for various valid password checking options.

Below is a program on isalpha() function.

```c
#include<stdio.h>
#include<ctype.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    /*
        As datatypes are int, hence all the variables store
        the ASCII values of the character on the rhs
    */
    int var1 = 'D';
    int var2 = '2';
    int var3 = 'a';
    int var4 = ' ';

    /*
        Returns true if the input parameter is an ASCII value
        of an alphabet character
    */
    if(isalpha(var1))
    {
        printf("\n var1 = |%c| is alphabet\n", var1);
    }
    else
    {
        printf("\n var1 =|%c| is not alphabet\n", var1);
    }

    if(isalpha(var2))
    {
        printf("\n var2 = |%c| is alphabet\n", var2);
    }
    else
    {
        printf("\n var2 =|%c| is not alphabet\n", var2);
    }

    if(isalpha(var3))
    {
        printf("\n var3 = |%c| is alphabet\n", var3);
    }
    else
    {
        printf("\n var3 =|%c| is not alphabet\n", var3);
    }

    if(isalpha(var4))
    {
        printf("\n var4 = |%c| is alphabet\n", var4);
    }
    else
    {
        printf("\n var4 =|%c| is not alphabet\n", var4);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
