# EX-NO-6-Pseudo-Random-Number

## NAME : Thaarakeshwar

## REG NUMBER : 212225040466


# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
~~~c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d ", random_number);
    }
    return 0;
}
~~~

# OUTPUT:

<img width="740" height="256" alt="image" src="https://github.com/user-attachments/assets/f6802bae-d4d3-4c33-8b59-c3fd1044e6b3" />


# RESULT:

The implementation of Pseudo Random Number technique using C program is executed sucessfully.
