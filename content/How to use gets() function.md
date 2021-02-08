---
title: "How to use gets() function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## How to use gets() function

Some of the important points about scanf() and gets() are:

Below is a program on use of gets().

gets() takes only a single line at a time i.e all the words before hitting \n(enter key).

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    char str[50];   // char array of size 50
    printf("Enter your complete name:\n\n\n");

    gets(str);
    printf("\n\nWelcome to C Programs  %s\n\n\n", str);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
