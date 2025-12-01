
# EX 42 C program to write a fuctions to perform push,pop,display,peek in stack using array.
## DATE: 6.10.25
## AIM:
To write a fuctions to perform push,pop,display,peek in stack using array.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a functions to perform push,pop,display,peek in stack using array. 
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

int stack[100];
int top = -1;
int n;

void push(int x)
{
    if (top == n - 1)
        return;
    top++;
    stack[top] = x;
}

int pop()
{
    if (top == -1)
        return -1;
    return stack[top--];
}

int peek()
{
    if (top == -1)
        return -1;
    return stack[top];
}

void display()
{
    int i;
    for (i = top; i >= 0; i--)
        printf("%d ", stack[i]);
}

int main()
{
    int choice, value;

    scanf("%d", &n);

    while (scanf("%d", &choice) != EOF)
    {
        if (choice == 1)
        {
            scanf("%d", &value);
            push(value);
        }
        else if (choice == 2)
        {
            pop();
        }
        else if (choice == 3)
        {
            printf("%d\n", peek());
        }
        else if (choice == 4)
        {
            display();
            break;
        }
    }

    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/d2596242-eca9-45e5-81c0-e3d4f5d9c88a)


## Result:
Thus the program was executed and the output was verified successfully.
