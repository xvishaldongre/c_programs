---
title: "Program to check whether a Number is a Palindrome"
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Program to check whether a Number is a Palindrome

Below is a program to check whether a number is a palindrome or not.

A palindrome is a number or a string which is similar when read from the front and from the rear. For example: 121 or Oppo etc.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    int a, b, c, s = 0;
    clrscr();
    printf("Enter a number:\t");
    scanf("%d", &a;);
    c = a;

   // the number is reversed inside the while loop.
   while(a > 0)
   {
      b = a%10;
      s = (s*10)+b;
      a = a/10;
   }

   // here the reversed number is compared with the given number.
   if(s == c)
   {
      printf("The number %d is a palindrome", c);
   }
   else
   {
      printf("The number %d is not a palindrome", c);
   }
  getch();
}
```
