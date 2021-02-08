---
title: "Program to find Armstrong Number between 1 to 500"
weight: 1
#date: 2021-02-05
draft: false
tags: ["numbers"]
---

## Program to find Armstrong Number between 1 to 500

An Armstrong number or Narcissistic number is a n digit number such that the sum of its digits raised to the nth power is equal to the number itself.

For example, Let's take an armstrong number: 153, which is 3 digit number, here 13 + 53 + 33 is 1 + 125 + 27 which is equal to 153.

Below is a program to find armstrong numbers between 1 to 500.

```c
#include<stdio.h>
#include<math.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n,sum,i,t,a;
    printf("\n\n\nThe Armstrong numbers in between 1 to 500 are : \n\n\n");

    for(i = 1; i <= 500; i++)
    {
        t = i;  // as we need to retain the original number
        sum = 0;
        while(t != 0)
        {
            a = t%10;
            sum += a*a*a;
            t = t/10;
        }

        if(sum == i)
        printf("\n\t\t\t%d", i);
    }

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Program to check whether a number is Armstrong Number

Below is a program to check whether a number is armstrong or not.

```c
#include<stdio.h>
#include<math.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    int n, sum = 0, c, t, a;

    printf("Enter a number:  ");
    scanf("%d", &n);

    t = n;  // as need to retain the original number
    while(n != 0)
    {
        a = n%10;
        sum += a*a*a;
        n = n/10;
    }

    printf("\n\n\n\t\t\tsum = %d", sum);

    if(sum == t)
        printf("\n\n\t\t%d is an armstrong number\n", t);
    else
        printf("\n\n\t\t%d is not an armstrong number\n", t);

    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
