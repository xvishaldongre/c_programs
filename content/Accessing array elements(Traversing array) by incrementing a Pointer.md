---
title: "Accessing array elements(Traversing array) by incrementing a Pointer"
weight: 1
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Accessing array elements(Traversing array) by incrementing a Pointer

Name of the array refers to the base address of the array.

Below is a program to access elements of an array using pointer increment.

```c
#include <stdio.h>

const int MAX = 3;  // Global declaration
int main()
{
	printf("\n\n\t\tC Programs\n\n\n");
	int var[] = {100, 200, 300};
    int i, *ptr;

    /*
        storing address of the first element
        of the array in pointer variable
    */
    ptr = var;

    for(i = 0; i < MAX; i++)
    {
        printf("\n\n\nAddress of var[%d] = %x ", i, ptr);
        printf("\nValue of var[%d] = %d ", i, *ptr);

       // move to the next location
        ptr++;
    }
	printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Traversing array elements by decrementing a Pointer

Below is a program to access elements of an array using pointer decrement.

```c
#include <stdio.h>

const int MAX = 3;  // Global declaration
int main()
{
	printf("\n\n\t\tC Programs\n\n\n");
	int var[] = {100, 200, 300};
    int i, *ptr;

    /*
        storing address of the last element
        of the array in pointer variable
    */
    ptr = &var[MAX-1];

	for(i = MAX; i > 0; i--)
    {
    	printf("\n\n\nAddress of var[%d] = %x ", i, ptr);
        printf("\nValue of var[%d] = %d ", i, *ptr);

		// move to the previous location
        ptr--;
	}
	printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
