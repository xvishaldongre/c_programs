---
title: "C Program to reverse a string using strrev() Function"
#date: 2021-02-05
draft: false
tags: ["string"]
---

## C Program to reverse a string using strrev() Function

In this program we will compare strings using the strrev() defined within the string.h library. It can be used to check if the string is pallindrome or not by using this function along with the strcmp() function.

Below is a program on strrev() function.

```c
#include<stdio.h>
#include<string.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj[1000];
    printf("\n\nstrrev(string): Function to reverse the string and storing in the same string.\n\n\n");
    printf("\n\nEnter the string: ");
    gets(aj);
    /*
        system defined function to reverse the string
        and storing in the same string
    */
    strrev(aj);
    printf("\n\nReverse of entered string is: %s", aj);
    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
