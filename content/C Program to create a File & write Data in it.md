---
title: "C Program to create a File & write Data in it"
#date: 2021-02-05
draft: false
tags: ["files_and_streams"]
---

## C Program to create a File & write Data in it

Below is a program to create a new file and then storing information in it.

You can add any information in the file, like we have added Name, Age and Salary for some employees, you can change the program as per your requirements.

You can even initialise a for loop, to add details of multiple employees to the file. All you have to do is, ask user for number of employees for which data has to be stored, run the for loop that many times and keep on adding the data to the file.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    FILE *fptr;
    char name[20];
    int age;
    float salary;

    /* open for writing */
    fptr = fopen("emp.txt", "w");

    if (fptr == NULL)
    {
        printf("File does not exist.\n");
        return;
    }
    printf("Enter the name:\n");
    scanf("%s", name);
    fprintf(fptr, "Name  = %s\n", name);

    printf("Enter the age:\n");
    scanf("%d", &age;);
    fprintf(fptr, "Age  = %d\n", age);

    printf("Enter the salary:\n");
    scanf("%f", &salary;);
    fprintf(fptr, "Salary  = %.2f\n", salary);

    fclose(fptr);
}
```
