---
title: "Checking for Odd and Even Numbers using Bitwise Operator"
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Checking for Odd and Even Numbers using Bitwise Operator

Below is a program to find whether a number is even or odd using bitwise operator.

x&1 returns true if the LSB(Least significant Bit) of binary representation of an integer x is 1. It returns false if the LSB or the Right most bit in a binary sequence is 0.

In binary representation of an integer, if LSB is 1 then it is odd and if LSB is 0 then it is even.

We have used a simple for loop to input numbers and show how to use the Bitwise operator. You can take input from user using scanf() and use th same logic to find if the input number is odd or even.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int x;
    for(x = 0; x <= 10; x++)
    {
        if(x&1) // if number is odd
            printf("\t\t\t%d is odd\n",x);
        else if(!(x&1)) // ! is used inside if to reverse the boolean value
            printf("\t\t\t%d is even\n",x);
    }

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Checking if inout number is Odd or Even without using %(Mod) Operator

Below is a program to find whether a number is even or odd without using %(Mod) operator.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n;
    printf("Enter a number:  ");
    scanf("%d",&n);

    if((n/2)*2 == n)
        printf("\n\n\t\t %d is Even\n", n);
    else
        printf("\n\n\t\t %d is Odd\n", n);

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
