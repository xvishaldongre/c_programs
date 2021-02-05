---
title: "C Programs to showcase the conversion between various Number Systems"
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C Programs to showcase the conversion between various Number Systems

Here we have multiple programs to showcase conversion between various Number systems like Binary to Decimal, Octal to Decimal, Decimal to Binary and we will even use recursion to help you understand how recursion can be used in such programs. So let's start.

## Program to convert Binary to Decimal Equivalent

Below is a program to convert binary number to its decimal equivalent.

```c
#include<stdio.h>
#include<math.h>

// Function prototype declaration
int binary_decimal(int n);

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n;
    char c;
    printf("Enter the binary number: ");
    scanf("%d", &n);
    printf("\n\n\nThe decimal equivalent of %d is  %d\n\n", n, binary_decimal(n)); // function calling
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

// Definition of the function to convert binary to decimal.
int binary_decimal(int n)
{
    int decimal = 0, i = 0, rem;
    while(n != 0)
    {
        rem = n%10;   // gives the digit at the units place
        n = n/10; // gives the number excluding its units digit
        /*
            pow is a system defined function that takes
            two integers as input parameters
        */
        decimal += rem*pow(2, i++);
    }
    /*
        return the decimal equivalent of the input
        binary number to the function call
    */
    return decimal;
}
```

## Program to convert Octal to Decimal Equivalent

Below is a program to convert octal number to its decimal equivalent.

%ld is the format specifier to input a long value.

```c
#include<stdio.h>
#include<stdio.h>
#include<math.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    long int octal, val, decimal = 0;
    int i = 0;
    printf("Enter any octal number: ");
    scanf("%ld", &val);
    octal = val;
    while(octal != 0)
    {
        /*
            i++ is post increment, where value is
            first assigned and then incremented
        */
      decimal += (octal % 10)*pow(8, i++);
      octal/=10;    // same as octal=octal/10
    }
    printf("\n\n\nEquivalent decimal value of %ld is %ld\n\n\n", val, decimal);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Program to convert Decimal to Binary Equivalent

Below is a program to convert decimal number to its binary equivalent without recursion.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n,c,k;
    printf("Enter an integer in decimal number system: ");
    scanf("%d", &n);

    // In 31 bit format
    printf("\n\n\nThe binary equivalent of decimal value %d is:", n);

    for(c = 31; c >= 0; c--)
    {
        k = n>>c;
        /*
            num&1 = returns true if the last digit of num is 1
            else false
        */
        if(k&1)
            printf("1");
        else
            printf("0");
    }
    printf("\n");
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Program to convert Decimal to Binary Equivalent using Recursion

Below is a program to convert decimal number to its binary equivalent with recursion:

```c
#include<stdio.h>

//Function prototype declarations
void decimal_binary(int );
void F(int );
void reverse(int );

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    int n;
    printf("\n\nEnter an integer in decimal number system: ");
    scanf("%d", &n);

    //In 31 bit format
    printf("\n\nThe binary equivalent of decimal value %d using decimal_binary method is: ", n);

    decimal_binary(n);  // function call

    printf("\n\nThe binary equivalent of decimal value %d using F() method is: ", n);
    F(n);   // function call
    printf("\n\nThe Reverse of the binary representation of value %d is: ", n);
    reverse(n); // function call
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}

// function definition
void decimal_binary(int i)
{
    if(i <= 1)
    printf("%d", i);   // to print in up to down format
    else
    {
        decimal_binary(i/2);
        printf("%d", i%2);
    }
}

void F(int j)
{
    if(j/2)
    {
        F(j/2);
    }
    printf("%d", j%2);
}

void reverse(int k)
{
    if(k <= 1)
        printf("%d", k);
    else
    {
        printf("%d", k%2);
        F(k/2);
    }
    printf("\n\n");
}
```
