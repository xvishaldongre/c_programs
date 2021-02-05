---
title: "Program to print Factorial of a Number"
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Program to print Factorial of a Number

```c
#include<stdio.h>
#include<conio.h>
void main()
{
   int fact, i, n;
   fact = 1;
   printf("Enter the number\t");
   scanf("%d" , &n;);
   for(i = 1; i <= n; i++)
   {
       fact = fact*i;
   }
   printf("Factorial of %d is %d", n , fact);
   getch();
}
```
