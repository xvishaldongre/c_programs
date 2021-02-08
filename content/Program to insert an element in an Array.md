---
title: "Program to insert an element in an Array"
weight: 1
#date: 2021-02-05
draft: false
tags: ["array"]
---

## Program to insert an element in an Array

Below is a simple program to insert an element in an array.

In the above program we take an array as user input and then ask the user for a new number that they wish to add to the original array, and the position where they want to add the new number.

The we shift the existing numbers from the index position to the end of the array one position to the right, therby vacating a space for the new element. And then we add the new number at the user specified position index.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int array[100], position, c, n, value;

    printf("\n\nEnter number of elements in array:");
    scanf("%d", &n);

    printf("\n\nEnter %d elements\n", n);
    for(c = 0; c < n; c++)
        scanf("%d", &array[c]);

    printf("\n\nEnter the location where you want to insert new element:  ");
    scanf("%d", &position);

    printf("\n\nEnter the value to insert: ");
    scanf("%d", &value);

    // shifting the elements from (position to n) to right
    for(c = n-1; c >= position-1; c--)
        array[c+1] = array[c];

    array[position - 1] = value;    // inserting the given value

    printf("\n\nResultant array is: ");
    /*
        the array size gets increased by 1
        after insertion of the element
    */
    for(c = 0; c <= n; c++)
        printf("%d  ", array[c]);

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
