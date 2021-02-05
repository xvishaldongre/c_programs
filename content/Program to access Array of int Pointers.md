---
title: "Program to access Array of int Pointers"
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Program to access Array of int Pointers

Below is a program to access an array of int pointers:

```c
#include <stdio.h>
/*
    Global declaration.
    Value of a const variable cannot be changed
    throughout the execution of program
*/
const int MAX = 5;

int main()
{

    printf("\n\n\t\tC Programs\n\n\n");

    int var[]={10, 20, 30, 40, 50}; // initializing an array(here var) of int pointers
    int i = 0;

    /*
        ptr is an array of int pointers i.e.
        it stores the address of each array element
    */
    int *ptr[MAX];

    for(i = 0; i < MAX; i++)
    {
        /*
            Assign the address of each of the array
            element to the ptr array
        */
        ptr[i] = &var[i];
    }

    for(i = 0; i < MAX; i++)
    {
        /*
            ptr[i] stores the address of the element var[i].
            Hence, *ptr[i] returns the value of the element
            stored at location ptr[i]
        */
        printf("Value of var[%d] = %i\n\n", i, *ptr[i]);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

```c
printf("Value of var[%d] = %i\n\n", i, *ptr[i]);
```

Here ptr[i] stores the address of the element var[i]. Hence, \*ptr[i] returns the value of the element stored at location var[i].

## Program to access Array of char pointers

Array of char pointers is used to access the complete string just using the address of the first char(base address) of each string.

Below is a program to access an array of char pointers.

```c
#include <stdio.h>
const int MAX = 4;  // Global declaration.

int main()
{

	printf("\n\n\t\tC Programs\n\n\n");

    char *names[] = {"Google", "Amazon", "Facebook", "Apple"}; // initializing an array(here names) of char pointers
    int i = 0;

    for(i = 0; i < MAX; i++)
    {
        printf("Value of names[%d] = %s\n\n", i, names[i]);
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

**Explanation:**

```c
printf("Value of names[%d] = %s\n\n",i,names[i]);
```

This statement is used for printing the complete name just using the pointer to the first character of each element of the names array.
