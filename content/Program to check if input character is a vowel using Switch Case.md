---
title: "Program to check if input character is a vowel using Switch Case"
weight: 1
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Program to check if input character is a vowel using Switch Case

Below is a program to check vowel using switch case.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    char ch;
    printf("Input a Character :  ");
    scanf("%c", &ch);

    switch(ch)
    {
        case 'a':
        case 'A':
        case 'e':
        case 'E':
        case 'i':
        case 'I':
        case 'o':
        case 'O':
        case 'u':
        case 'U':
            printf("\n\n%c is a vowel.\n\n", ch);
            break;
        default:
            printf("%c is not a vowel.\n\n", ch);
    }
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
