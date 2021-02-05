---
title: "Program to reverse the case of input character"
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Program to reverse the case of input character

Below is a program to reverse the case of input character.

getchar() is similar to scanf().

islower() is system defined function under ctype.h header file to check if the character is in lowercase or not.

toupper() converts the input parameter into equivalent uppercase char.

putchar() is similar to printf().

```c
#include<stdio.h>
#include<ctype.h> // to use system defined function islower & toupper

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    char alphabet;
    printf("Enter an alphabet : ");
    putchar('\n');  // to move to next Line

    alphabet=getchar();

    printf("\n\nReverse case of %c is :  ",alphabet);

    if(islower(alphabet))
        putchar(toupper(alphabet));

    else
        // must be an uppercase character
        printf("%c",tolower(alphabet)) ;

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
