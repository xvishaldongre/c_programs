---
title: "Program to find Largest and Smallest Element in an Array"
weight: 1
#date: 2021-02-05
draft: false
tags: ["array"]
---

## Program to find Largest and Smallest Element in an Array

Below is a program to find the largest and smallest elements in array.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int a[50], size, i, big, small;

    printf("\nEnter the size of the array: ");
    scanf("%d", &size);

    printf("\n\nEnter the %d elements of the array: \n\n", size);
    for(i = 0; i < size; i++)
    scanf("%d", &a[i]);

    big = a[0]; // initializing
    /*
        from 2nd element to the last element
        find the bigger element than big and
        update the value of big
    */
    for(i = 1; i < size; i++)
    {
        if(big < a[i])   // if larger value is encountered
        {
            big = a[i]; // update the value of big
        }
    }
    printf("\n\nThe largest element is: %d", big);

    small = a[0];   // initializing
    /*
        from 2nd element to the last element
        find the smaller element than small and
        update the value of small
    */
    for(i = 1; i < size; i++)
    {
        if(small>a[i])   // if smaller value is encountered
        {
            small = a[i];   // update the value of small
        }
    }
    printf("\n\nThe smallest element is: %d", small);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
