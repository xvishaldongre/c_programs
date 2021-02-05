---
title: "ASCII value of Character"
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## ASCII value of Character

Below is a program to find ASCII value of any input character.

%c is the format specifier to take character as input

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    char c;
    printf("Enter a character : ");
    scanf("%c" , &c);
    printf("\n\nASCII value of %c = %d",c,c);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
