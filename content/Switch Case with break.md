---
title: "Switch Case with break"
#date: 2021-02-05
draft: false
tags: ["Basic Programs"]
---

## Switch Case with break

Below is a program on switch case with break.

switch() can only contain char and int.

break is used to exit from switch statement.

switch case can be without default case.

Another piece of information here is that a char variable is always initialized within ''(single quotes).

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    // Local Variable Definition
    char grade;
    printf("Enter your grade:\n");
    scanf("%c", &grade);

    switch(grade)
    {
        case 'A':
            printf("Excellent\n");
            break;
        case 'B':
            printf("Keep it up!\n\n");
            break;
        case 'C':
            printf("Well done\nbreak keyword takes execution to exit the switch case\n\n");
            break;
        case 'D':
            printf("You passed\n");
            break;
        case 'F':
            printf("Better luck next time\n");
            break;
        default:
            printf("Invalid grade\n");
    }
    printf("Your grade is %c\n",grade);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```

## Switch Case without break

Below is a program on switch case without break.

If there is no break statement then the cases following the matched case other than default will get executed.

```c
#include<stdio.h>

int main()
{
    printf("\n\n\t\tC Programs\n\n\n");

    /* Local Variable Definition */
    char grade;
    printf("Enter your grade:\n");
    scanf("%c", &grade);

    switch(grade)
    {
        case 'A':
            printf("Excellent\n");
        case 'B':
            printf("\n\n\nKeep it up!\n\nNo break statement\n\nHence all the case following this(but not the ones above this) except the default case will get executed !\n\n");
        case 'C':
            printf("\n\n\t\tCase C : Well done !\n\n");
        case 'D':
            printf("\t\tCase D : You passed!\n\n");
        case 'F':
            printf("\t\tCase E : Better luck next time\n\n\n");
        default:
            printf("\t\tDefault Case : Invalid grade\n\n\n");
    }
    printf("Your grade is %c\n",grade);
    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
```
