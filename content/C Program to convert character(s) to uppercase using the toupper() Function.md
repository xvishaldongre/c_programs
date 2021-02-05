---
title: "C Program to convert character(s) to uppercase using the toupper() Function"
#date: 2021-02-05
draft: false
tags: ["CTYPE.H"]
---

## C Program to convert character(s) to uppercase using the toupper() Function

In this program we will convert all the characters of an input string to uppercase characters. We will be using a system defined function toupper() defined under the ctype.h library.

This can also be achieved by subtracting 32 from each lowercase character to get its equivalent uppercase format.

Below is the program on toupper() function. Try running the program and you will see all the explanation printed on the output screen. Yay!

```c
#include<stdio.h>
#include<ctype.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    printf("putchar() is used to print a single character at a time on the console.\n\n\n");
    printf("toupper() takes a character as an input and converts it into an equivalent upper-case character.\n\n\n");
    printf("This can also be achieved by subtracting 32 from each lowercase character\n to get its equivalent uppercase format. \n\n\n");
    printf("As we know ASCII value of a = %d and that of A = %d.\n\n\n ",'a','A');
    printf("\n\nLet's first get the concept:\n\n\n ");
    printf("\n\nThe uppercase equivalent of letter 'a' is %c.\n\n ",'a'-32);

    int aj = 0;
    char mj[] = " \n\nKeep learning, as what you know will never be enough!\n\n";

    while(mj[aj])   // until string terminates
    {
        // converting one character at a time
        putchar(toupper(mj[aj]));
        aj++;
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
