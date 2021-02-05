---
title: "C Program to convert Temparature in Celsius to Fahrenheit"
#date: 2021-02-05
draft: false
tags: ["important_concepts"]
---

## C Program to convert Temparature in Celsius to Fahrenheit

## C Program to convert Temparature in Celsius to Fahrenheit

Below is a program for temperature conversion from Celsius to Fahrenheit. All we have to do is use the simple formula in our program, which is, if a temparature value is in Celsius, multiply it with 1.8 or 9/5 and add 32 to the result, this will give the equivalent Fahrenhiet value.

To convert a temparature in Fahrenheit to Celsius, the formula will be, to subtract 32 from the value and then multiply it with 0.5556 or 5/9

So all you have to do is replace the conversion formula in the avove program. Go ahead and try it out yourself.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    float celsius, fahrenheit;
    printf("\n\nEnter temperature in Celsius: ");
    scanf("%f", &celsius);

    fahrenheit = (1.8*celsius) + 32;

    printf("\n\n\nTemperature in Fahrenheit is: %f ", fahrenheit);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
