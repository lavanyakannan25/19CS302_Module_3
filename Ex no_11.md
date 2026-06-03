# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE:
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1. Start the program. 
2. Create a function with no arguments that reads a decimal number from the user.
3. Inside the function, convert the number to binary using a loop and store the binary digits.
4. Return 0 from the function after displaying the binary equivalent. 
5. Call the function from main() and end the program.  

## Program:
```
/*
Program to C Program to convert a given decimal value to binary using function without arguments with return type.
*/
#include <stdio.h>

int convertToBinary() {
    int num, binary[32], i = 0;
    scanf("%d", &num);

    if(num == 0) {
        printf("Binary: 0\n");
        return 0;
    }

    while(num > 0) {
        binary[i++] = num % 2;
        num /= 2;
    }

    printf("Binary: ");
    for(int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }
    printf("\n");

    return 0;
}

int main() {
    convertToBinary();
    return 0;
}
```

## Output:
<img width="381" height="165" alt="image" src="https://github.com/user-attachments/assets/74010053-da27-4ee8-9ec3-8f598f74c8f1" />



## Result:
Thus the program was executed and the output was verified successfully.
