---
title: "Program to print the Fibonacci Series"
weight: 1
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Program to print the Fibonacci Series

```c
#include<stdio.h>
#include<conio.h>

void fibonacci(int num);
void main()
{
    int num = 0;
    clrscr();
    printf("Enter number of terms\t");
    scanf("%d", &num);
    fibonacci(num);
    getch();
}

void fibonacci(int num)
{
   int a, b, c, i = 3;
   a = 0;
   b = 1;
   if(num == 1)
   printf("%d",a);

   if(num >= 2)
   printf("%d\t%d",a,b);

   while(i <= num)
   {
      c = a+b;
      printf("\t%d", c);
      a = b;
      b = c;
      i++;
   }
}
```
