---
title: "C Program to check for whitespace using isspace() Function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["CTYPE.H"]
---

## C Program to check for whitespace using isspace() Function

In this program we will check white spaces as well as tabs. We will be using a system defined function isspace() defined under the ctype.h library.

This can be done using if-else block, condition being the ASCII value of the space character.

This method is used for various valid password checking options as well as the variable names in the C compiler as valid names shall not contain white spaces.

Below is a program on isspace() function.

int always considers the last character as valid, of a given series of characters.

Leading spaces of a character are not considered as spaces.

Trailing spaces are considered as spaces.

```c
#include<stdio.h>
#include<ctype.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int var1 = '   d';
    int var2 = '2';
    int var3 = '\t';
    int var4 = 'a  ';

    /*
        Returns true if the input parameter is an ASCII value
        of a white-space character
    */
    if(isspace(var1))
    {
        printf("\n var1 = |%c| is a white-space character\n", var1);
    }
    else
    {
        printf("\n var1 =|%c| is not a white-space character\n", var1);
    }

    if(isspace(var2))
    {
        printf("\n var2 = |%c| is a white-space character\n", var2);
    }
    else
    {
        printf("\n var2 =|%c| is not a white-space character\n", var2);
    }

    if(isspace(var3))
    {
        printf("\n var3 = |%c| is a white-space character\n", var3);
    }
    else
    {
        printf("\n var3 =|%c| is not a white-space character\n", var3);
    }

    if(isspace(var4))
    {
        printf("\n var4 = |%c| is a white-space character\n", var4);
    }
    else
    {
        printf("\n var4 =|%c| is not a white-space character\n", var4);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
