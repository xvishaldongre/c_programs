---
title: "C Program to find the Size of any File"
weight: 1
#date: 2021-02-05
draft: false
tags: ["files_and_streams"]
---

## C Program to find the Size of any File

We will be using fseek() and ftell() functions to find the size of the file. There are others ways to find the file size as well, like looping on the whole content of file and finding out the size, but the File Handling functions makes it a lot easier.

Below is a program to find size of file.

```c
#include<stdio.h>
#include<conio.h>

void main()
{
    FILE *fp;
    char ch;
    int size = 0;

    fp = fopen("MyFile.txt", "r");
    if (fp == NULL)
    {
        printf("\nFile unable to open...");
    }
    else
    {
        printf("\nFile opened...");
    }
    fseek(fp, 0, 2);    /* File pointer at the end of file */
    size = ftell(fp);   /* Take a position of file pointer in size variable */
    printf("The size of given file is: %d\n", size);
    fclose(fp);
}
```
