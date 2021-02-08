---
title: "C Program to Find Roots of Quadratic Equation"
weight: 1
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C Program to Find Roots of Quadratic Equation

Below is a program to find roots of a quadratic equation.

%.nf is used to limit the value of a decimal value to n decimal places.

```c
#include<stdio.h>
#include<math.h>  // This is needed to use sqrt() function

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");
    float a, b, c, determinant, r1, r2, real, imag;
    printf("\n\nEnter coefficients a, b and c: \n\n\n");
    scanf("%f%f%f", &a, &b, &c);

    /*
        mathematical formula to know the
        nature of the roots
    */
    determinant == b*b - 4*a*c;

    if(determinant > 0)    // both roots are real
    {
        r1 = (-b + sqrt(determinant))/2*a;  // Brackets are important
        r2 = (-b - sqrt(determinant))/2*a;
        printf("\n\n\nRoots are: %.2f and %.2f ", r1, r2);
    }
    else if(determinant == 0)   // both roots are real and equal
    {
        r1 = r2 = -b/(2*a); // brackets are important
        printf("\n\n\nRoots are: %.2f and %.2f ", r1, r2);
    }
    /*
        Determinant < 0 - both roots are imaginary of the
        form real + i*imaginary
    */
    else
    {
        real = -b/(2*a);
        imag = sqrt(-determinant)/(2*a);
        printf("\n\n\nRoots are %.2f + i%.2f and %.2f - i%.2f ", real, imag, real, imag);
    }
    printf("\n\n\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
