---
title: "Program to find Palindrome using Recursion"
weight: 1
#date: 2021-02-05
draft: false
tags: ["recursion"]
---

## Program to find Palindrome using Recursion

A Palindrome is a sequence that if reversed looks identical to the original sequence Eg : abba, level, 999 etc.

Below is a simple C program to find whether the user input number is a palindrome or not using recursion:

```c
#include<stdio.h>

// declaring the recursive function
int isPal(int );

/*
    global declaration to use the same value
    in both the functions
*/
int n;

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int palindrome;
    printf("\n\nEnter a number to check for Palindrome: ");
    scanf("%d", &n);
    palindrome = isPal(n);
    if(palindrome == 1)
        printf("\n\n\n%d is palindrome\n\n", n);
    else
        printf("\n\n\n%d is not palindrome\n\n", n);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

int isPal(int aj)
{
    static int sum = 0;
    if(aj != 0)
    {
        sum = sum *10 + aj%10;
        isPal(aj/10);   // recursive call same as while(n!=0) using loop
    }
    else if(sum == n)
        return 1;
    else
        return 0;
}
```
