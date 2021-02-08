---
title: "Pointer Comparison in C"
weight: 1
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Pointer Comparison in C

In C language pointers can be compared if the two pointers are pointing to the same array.

All relational operators can be used for pointer comparison, but a pointer cannot Multiplied or Divided.

Below is a program on pointer comparison for same type of pointer:

```c
#include <stdio.h>

int main()
{
    int *ptrA,*ptrB;

    ptrA = (int *)1;
    ptrB = (int *)2;

    if(ptr2 > ptr1)
        printf("PtrB is greater than ptrA");

return(0);
}
```

Below is a program on pointer comparison for different type of pointer:

```c
#include <stdio.h>

int main()
{
    int *ptrA;
    float *ptrB;

    ptrA = (int *)1000;
    ptrB = (float *)2000;

    if(ptrB > ptrA)
       printf("PtrB is greater than ptrA");

    return(0);
}
```
