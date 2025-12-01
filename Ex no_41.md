
# EX 41 C program to write a function to find the peek of stack using array.
## DATE: 6.10.25
## AIM:
To write a function to find the peek of stack using array.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a function to find the peek of stack using array. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End.  

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

float stack[100];
int top = -1;

void push(float x)
{
    top++;
    stack[top] = x;
}

float peek()
{
    return stack[top];
}

int main()
{
    float a, b, c;
    
    scanf("%f %f %f", &a, &b, &c);

    push(a);
    push(b);
    push(c);

    printf("%.2f", peek());

    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/e6990a19-fb3b-459d-b7cb-ed4c69b331cf)


## Result:
Thus the program was executed and the output was verified successfully.
