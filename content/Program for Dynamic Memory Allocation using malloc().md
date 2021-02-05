---
title: "Program for Dynamic Memory Allocation using malloc()"
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Program for Dynamic Memory Allocation using malloc()

Below is a program on dynamic memory allocation using malloc() and clearing out memory space using free().

sizeof() returns the number of bytes occupied by any datatype, in this case by an integer.

```c
#include <stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n, i, *ptr, sum = 0;

    printf("\n\nEnter number of elements: ");
    scanf("%d", &n);

    // dynamic memory allocation using malloc()
    ptr = (int *) malloc(n*sizeof(int));

    if(ptr == NULL) // if empty array
    {
        printf("\n\nError! Memory not allocated\n");
        return 0;   // end of program
    }

    printf("\n\nEnter elements of array: \n\n");
    for(i = 0; i < n; i++)
    {
        // storing elements at contiguous memory locations
        scanf("%d", ptr+i);
        sum = sum + *(ptr + i);
    }

    // printing the array elements using pointer to the location
    printf("\n\nThe elements of the array are: ");
    for(i = 0; i < n; i++)
    {
        printf("%d  ",ptr[i]);    // ptr[i] is same as *(ptr + i)
    }

    /*
        freeing memory of ptr allocated by malloc
        using the free() method
    */
    free(ptr);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```