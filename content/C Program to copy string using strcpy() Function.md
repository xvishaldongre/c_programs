---
title: "C Program to copy string using strcpy() Function"
#date: 2021-02-05
draft: false
tags: ["string"]
---

## C Program to copy string using strcpy() Function

In this program we will copy one string into another, using the strcpy() method defined under the string.h library.

strcpy(destination, source) is a system defined method used to copy the source string into the destination variable.

Below is a program on strcpy() function.

```c
#include<stdio.h>
#include<string.h>    // for using strcpy() function

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char mj[100];
    char aj[100];
    printf("\n\nstrcpy(destination, source): is a system defined method used to copy the source string into the destination.\n\n");
    printf("\n\nEnter the string: ");
    gets(aj);
    strcpy(mj, aj);
    printf("\n\nThe copied string is: %s\n\n", mj);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## C Program to copy string without strcpy() function

What if you do not want to use the system defined function?

While initializing a string, there is no need to put a null character at the end, as the compiler provides it automatically.

For example, char aj[] = "aditya"; is a correct statement. However while copying one string into another, terminating the destination string with a null character is mandatory, to use it in future.

Below is a program for copying string without the use of strcpy() function.

```c
#include<stdio.h>

void stringCopy(char[], char[]);    // function prototype declaration

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    char aj[100], mj[100];
    printf("\n\nEnter 1st string: ");
    gets(aj);
    stringCopy(aj, mj); // function call
    printf("\n\nThe copied string is: %s\n\n", mj);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

void stringCopy(char a[], char b[]) // function definition
{
    int i = 0;
    while(a[i] != '\0')
    {
        b[i] = a[i];
        i++;
    }

    /*
        The string must always terminate with
        a '\0' - null character
    */
    b[i] =' \0';    // most important step
}
```
