---
title: "Program to find Sum of Digits of a Number"
#date: 2021-02-05
draft: false
tags: ["loops"]
---

## Program to find Sum of Digits of a Number

Below is a program for sum of digits of a number.

```c
#include<stdio.h>

int main()
{
	printf("\n\n\t\tC Programs\n\n\n");

	int n, sum = 0, c, remainder;

    	printf("Enter the number you want to add digits of:  ");
    	scanf("%d", &n);

	while(n != 0)
    	{
        	remainder = n%10;
        	sum += remainder;
        	n = n/10;
    	}

    	printf("\n\nSum of the digits of the entered number is  =  %d\n\n", sum);
    	printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    	return 0;
}
```
