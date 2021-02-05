---
title: "Null Pointer Program"
#date: 2021-02-05
draft: false
tags: ["pointers"]
---

## Null Pointer Program

Null pointer is a special reserved value of a pointer. A pointer of any type has this reserved value. Formally, each specific pointer type(int _, char _, etc) has its own dedicated null-pointer value. Conceptually, when a pointer has that Null value it is not pointing anywhere.

Void pointer is a specific pointer type. void \* which is a pointer that points to some data location in storage, which doesn't have any specific type.

Null pointer is a value whereas, Void pointer is a type.

Below is a program on NULL pointer.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int *ptr = NULL;    // ptr is a NULL pointer

    printf("\n\n The value of ptr is: %x ", ptr);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
