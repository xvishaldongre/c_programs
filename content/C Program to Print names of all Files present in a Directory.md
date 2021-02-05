---
title: "C Program to Print names of all Files present in a Directory"
#date: 2021-02-05
draft: false
tags: ["files_and_streams"]
---

## C Program to Print names of all Files present in a Directory

dirent.h header file contains variables and functions related to directory streams.

Below is a program to print the names of all the files in a directory.

We can also take the directory name as input from the user, and can also create a simple C program to search for a particular file in a directory.

```c
#include<stdio.h>
#include<dirent.h>

int main(void)
{
    DIR *d;
    struct dirent *dir;
    d = opendir(".");
    if (d)
    {
        while ((dir = readdir(d)) != NULL)
        {
            printf("%s\n", dir->d_name);
        }
        closedir(d);
    }
    return(0);
}
```
