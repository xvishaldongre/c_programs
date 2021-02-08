---
title: "C Program to compare two strings using strcmp() Function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["string"]
---

## C Program to compare two strings using strcmp() Function

In this program we will compare strings using strcmp() function defined in the string.h library.

strcmp(a, b) returns 0 if both the strings a and b are exactly same else returns -1.

It is case sensitive so 'ABC' and 'abc' are considered to be different strings. It can be used with with strrev() function(function to reverse a string) to check whether a given string is a Pallindrome or not.

Below is a program on strcmp() function.

```c
#include<stdio.h>
#include<string.h>    // for strcmp() function

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj1[100], aj2[100];
    int compare;

    printf("\n\nstrcmp(a,b) returns : 0 if both the strings are exactly same and -1 otherwise.\n\n\n");
    printf("\n\nstrcmp(a,b) is Case Sensitive.\n\n\n");

    printf("\n\nEnter 1st string: ");
    gets(aj1);

    printf("\n\nEnter 2nd string: ");
    gets(aj2);

    compare = strcmp(aj1, aj2);
    if(compare == 0)
        printf("\n\nBoth the strings are exactly same.\n\n");
    else
        printf("\n\nBoth the strings are different.\n");

    printf("\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## C Program to compare strings without strcmp() function

Below is a program to compare strings, without the use of strcmp() function.

```c
#include<stdio.h>

int stringCompare(char[], char[]);  // function prototype declaration

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj1[100], aj2[100];
    int compare;

    printf("\n\nEnter 1st string: ");
    scanf("%s", aj1);

    printf("\n\nEnter 2nd string: ");
    scanf("%s", aj2);

    compare = stringCompare(aj1, aj2);  // function call

    if(compare == 1)
        printf("\n\nBoth the strings are exactly same.\n\n");
     else
        printf("\n\nBoth the strings are different.\n");

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

int stringCompare(char mj1[], char mj2[])  // function definition
{
    int i = 0, flag = 0;
    while(mj1[i] != '\0' && mj2[i] != '\0') // until atleast one string ends
    {
        /*
            Even if they differ by a single character,
            don't iterate further
        */
        if(mj1[i] != mj2[i])
        {
            flag = 1;
            break;
        }
        i++;
    }

    /*
        If all the characters are sequentially same as well as
        both strings have ended
    */
    if(flag == 0 && mj1[i] == '\0' && mj2[i] == '\0')
        return 1;
    else
        return 0;
}
```
