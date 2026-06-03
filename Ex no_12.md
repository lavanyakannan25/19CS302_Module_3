# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE:
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1. Start the program and define a function with arguments and no return type.
2. Read a number from the user in main().
3. Pass the number as an argument to the function.
4. In the function, check if the number is divisible by any number from 2 to n/2. 
5. Print whether the number is prime or not from the function.  

## Program:
```
/*
C program to check whether the given number is prime or not using function without return type and with arguments.
*/
#include <stdio.h>

void checkPrime(int num)
{
    int i, isPrime = 1;

    if(num <= 1)
    {
        printf("%d is not a prime number.\n", num);
        return;
    }

    for(i = 2; i <= num / 2; i++)
    {
        if(num % i == 0)
        {
            isPrime = 0;
            break;
        }
    }

    if(isPrime)
    {
        printf("%d is a prime number.\n", num);
    }
    else
    {
        printf("%d is not a prime number.\n", num);
    }
}

int main()
{
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    checkPrime(number);

    return 0;
}
```

## Output:

<img width="379" height="205" alt="image" src="https://github.com/user-attachments/assets/a3caf0b0-1720-4bdc-9d8e-6e9ab507e55f" />


## Result:
Thus the program was executed and the output was verified successfully.
