---
title: "C program to check for punctuation characters using the ispunct() Function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["CTYPE.H"]
---

## C program to check for punctuation characters using the ispunct() Function

In this program we will check if a character is a punctuation character or not. We will be using a system defined function ispunct() defined under the ctype.h library.

Again, this can be done using if-else block condition using the range of ASCII values of punctuation characters. This method is used for various valid password checking options where atleast one punctuation character is mandatory.

Below is a program on ispunct() function.

```c
#include<stdio.h>
#include<ctype.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    /*
        As datatypes are int, hence all the variables store the
        ASCII values of the character on the rhs
    */
    int var1 = 'D';
    int var2 = '2';
    int var3 = '/';
    int var4 = ',';

    /*
        Returns true if the input parameter is an ASCII value
        of a punctuation character
    */
    if(ispunct(var1))
    {
        printf("\n var1 = |%c| is a punctuation character\n", var1);
    }
    else
    {
        printf("\n var1 =|%c| is not a punctuation character\n", var1);
    }

    if(ispunct(var2))
    {
        printf("\n var2 = |%c| is a punctuation character\n", var2);
    }
    else
    {
        printf("\n var2 =|%c| is not a punctuation character\n", var2);
    }

    if(ispunct(var3))
    {
        printf("\n var3 = |%c| is a punctuation character\n", var3);
    }
    else
    {
        printf("\nvar3 =|%c| is not a punctuation character\n", var3);
    }

    if(ispunct(var4))
    {
        printf("\n var4 = |%c| is a punctuation character\n", var4);
    }
    else
    {
        printf("\n var4 =|%c| is not a punctuation character\n", var4);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
