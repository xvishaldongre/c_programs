---
title: "Difference between strlen() and sizeof() function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["string"]
---

## Difference between strlen() and sizeof() function

Below is a program on strlen() and sizeof() function.

strlen() is a system defined function that does not consider the null character \0.

```c
#include<stdio.h>
#include<conio.h>
#include<string.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj[] = "C Programs";
    int length1, length2;

    length1 = sizeof(aj);
    length2 = strlen(aj);

    // need to put in backslash infront to print the quote symbol
    printf("\n\n\nsizeof() of string \"C Programs\" returns %d and strlen() returns %d.", length1, length2);
    printf("\n\n\nsizeof() also considers \'\\0\' as a part of the string.\n");
    printf("\n\n\nHence, for a predefined string: sizeof() = strlen() + 1 \n");
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
