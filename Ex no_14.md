# EX 14 C program to delete first element in an array.
## DATE:
## AIM:
To write a C program to delete first element in an array.

## Algorithm
1. Start the program and declare an array with its size.
2. Read the size and elements of the array from the user.
3. Shift all elements one position to the left starting from index 1.
4. Decrease the size of the array by 1. 
5. Display the updated array without the first element.  

## Program:
```
/*
Program to delete first element in an array. 
*/
#include <stdio.h>

int main()
{
    int arr[100], n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter the elements:\n");
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    // Shift elements to delete the first one
    for(i = 0; i < n - 1; i++)
    {
        arr[i] = arr[i + 1];
    }

    n--; // Reduce size after deletion

    printf("Array after deleting the first element:\n");
    for(i = 0; i < n; i++)
    {
        printf("%d ", arr[i]);
    }

    printf("\n");
    return 0;
}

```

## Output:

<img width="691" height="145" alt="image" src="https://github.com/user-attachments/assets/454c70a6-0824-43f6-b7a8-76d601d64257" />


## Result:
Thus the program was executed and the output was verified successfully.
