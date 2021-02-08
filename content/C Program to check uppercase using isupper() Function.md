---
title: "C Program to check uppercase using isupper() Function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["CTYPE.H"]
---

## C Program to check uppercase using isupper() Function

In this program we will check whether a character is in upper-case or not. We will be using a system defined function isupper() defined under the ctype.h library.

This can also be done using if-else blocks condition using the range of the ASCII values of the upper-case alphabets which is 65 to 90.

This method is used for various valid password checking options where atleast one upper-case character is mandatory.

Below is a program on isupper() function.

```c
#include<stdio.h>
#include<ctype.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    /*
        As datatypes are int, hence all the variables store
        the ascii values of the character on the rhs
    */
    int var1 = 'D';
    int var2 = 65;
    int var3 = 'a';
    int var4 = 98;

    printf("Range of ASCII values of upper-case characters is 65 to 90\n\n");
    printf("\n\nintegers and characters are interconvertible using the ASCII values.\n\n\nThe only condition is that correct format specifier shall be used \nas per what is desired to be printed.\n\n\nThe characters must be initialized in between single quotes. \' \'\n\n");

    /*
        Returns true if the input parameter is an ascii value
        of a upper-case alphabet
    */
    if(isupper(var1))
    {
        printf("\n var1 = |%c| is a upper-case character\n", var1);
    }
    else
    {
        printf("\n var1 =|%c| is not a upper-case character\n", var1);
    }

    if(isupper(var2))
    {
        printf("\n var2 = |%c| is a upper-case character\n", var2);
    }
    else
    {
        printf("\n var2 =|%c| is not a upper-case character\n", var2);
    }

    if(isupper(var3))
    {
        printf("\n var3 = |%c| is a upper-case character\n", var3);
    }
    else
    {
        printf("\n var3 =|%c| is not a upper-case character\n", var3);
    }

    if(isupper(var4))
    {
        printf("\n var4 = |%c| is a upper-case character\n", var4);
    }
    else
    {
        printf("\n var4 =|%c| is not a upper-case character\n", var4);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
