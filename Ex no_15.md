# EX 15 C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.
## DATE:
## AIM:
To write a C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.

## Algorithm
1. Start the program and declare an integer array and size variable.
2. Read the number of elements and the array values from the user.
3. Traverse the array and check if each element is even.
4. If even, replace it with the character 'E' using a separate array. 
5. Display the updated array.  

## Program:
```
/*
Program that reads a one-dimensional array of integers and replaces all even elements with 'E'.
*/
#include <stdio.h>

int main()
{
    int arr[100], n, i;
    char modified[100];

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter the elements:\n");
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < n; i++)
    {
        if(arr[i] % 2 == 0)
        {
            modified[i] = 'E';
        }
        else
        {
            modified[i] = arr[i]; 
        }
    }

    printf("Modified array:\n");
    for(i = 0; i < n; i++)
    {
        if(modified[i] == 'E')
        {
            printf("E ");
        }
        else
        {
            printf("%d ", modified[i]);
        }
    }

    printf("\n");
    return 0;
}
```

## Output:
<img width="372" height="289" alt="image" src="https://github.com/user-attachments/assets/e67d063a-9aa0-4cc9-929c-10cbcd431928" />



## Result:
Thus the program was executed and the output was verified successfully.
