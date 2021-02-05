---
title: "C Program to Display the current Date and Time"
#date: 2021-02-05
draft: false
tags: ["miscellaneous"]
---

## C Program to Display the current Date and Time

Below is the program to display current date and time.

#include<time.h> is used for time and ctime function and time_t datatype.

```c
#include<stdio.h>
#include<time.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    time_t t;   // not a primitive datatype
    time(&t);

    printf("\nThis program has been writeen at (date and time): %s", ctime(&t));

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
