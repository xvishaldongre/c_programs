---
title: "C gets() and strlen() function"
#date: 2021-02-05
draft: false
tags: ["string"]
---

## C gets() and strlen() function

Some important points about gets() and scanf() methods are:

Below is a program on gets() and strlen() function.

```c
#include<stdio.h>
#include<string.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char a[100];
    int length;

    printf("\n\nEnter a string you wish to calculate the length of :   ");
    /*
        to take a single string (including spaces)
        as input at a time
    */
    gets(a);
    /*
        Return the length of the string
        or the number of characters in the string
    */
    length = strlen(a);

    printf("\n\nThe length of the input string is: %d\n\n", length);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## C Program to find Length of a string without strlen() function

Below is a program to find the length of a string without the use of strlen() function.

You must be wondering why we have not added any statement to our for loop. It's because we are traversing our string until we encounter \0 and are doing i++ every time, hence we do not have to do anything else inside the loop, as the value of i will be equal to the length of the string by the time we encounter the \0 character.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj[1000];
    int i = 0;

    printf("\n\nEnter the string: ");
    gets(aj);

    // \0 marks the end of the string
    for(i = 0; aj[i] != '\0' ;i++);   // updation is done after checking condition

    printf("\n\nThe length of the input string is :  %d", i);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
