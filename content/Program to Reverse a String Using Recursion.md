---
title: "Program to Reverse a String Using Recursion"
weight: 1
#date: 2021-02-05
draft: false
tags: ["recursion"]
---

## Program to Reverse a String Using Recursion

Below is a program to reverse a user input string using recursion in C language.

```c
#include<stdio.h>
#include<conio.h>

// declaring recursive function
char* reverse(char* str);

void main()
{
    int i, j, k;
    char str[100];
    char *rev;
    printf("Enter the string:\t");
    scanf("%s", str);
    printf("The original string is: %s\n", str);
    rev = reverse(str);
    printf("The reversed string is: %s\n", rev);
    getch();
}

// defining the function
char* reverse(char *str)
{
    static int i = 0;
    static char rev[100];
    if(*str)
    {
        reverse(str+1);
        rev[i++] = *str;
    }
    return rev;
}
```
