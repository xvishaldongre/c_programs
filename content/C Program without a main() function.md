---
title: "C Program without a main() function"
weight: 1
#date: 2021-02-05
draft: false
tags: ["miscellaneous"]
---

## C Program without a main() function

Below is a program without main().

In the below program, main() function is there, but hidden using the preprocessors.

As you can see in the second line, #define decode() function is used, which holds a character combination of m,a,i,n and is followed by ##m##a##i##n.

Here ## operator is used to merge the characters in the order mentioned using ##, which is main

In the 3rd line #define go decode(m,a,i,n) as we have specified the characters in same order, the decode function will assign value main for go.

```c
#include<stdio.h>
//Need to include the following statements in same manner
#define decode(m,a,i,n) m##a##i##n
#define go decode(m,a,i,n)

int go()
{
    printf("\n\n\t\tC Programs\n\n\n");
    printf("You have just executed your first program without making use of main() function!\n");
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

We can use different words and combination here, like

```c
#define decode(s,t,u,m,p,e,d) m##s##u##t
#define go decode(a,n,i,m,a,t,e)
```

## Using macro to define main

```c
#include<stdio.h>
#define go main
int go(void)
{
    printf("Welcome to C Programs");
    return 0;
}
```

This is is the simplest technique, where all we have done is provided our main() function with a different name, which is set the main before the program is executed.

## Using Token-Pasting operator

```c
#include<stdio.h>
#define go m##a##i##n
int go(void)
{
    printf("Welcome to C Programs");
    return 0;
}
```
