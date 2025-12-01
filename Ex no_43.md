
# EX 43 C program to Write a function to display queue elements using array.
## DATE: 6.10.25
## AIM:
To Write a function to display queue elements using array.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a function to display queue elements using array. 
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

char queue[100];
int front = -1, rear = -1;

void enqueue(char x)
{
    if (rear == -1)
    {
        front = rear = 0;
        queue[rear] = x;
    }
    else
    {
        rear++;
        queue[rear] = x;
    }
}

void display()
{
    if (front == -1)
    {
        printf("no elements to display");
        return;
    }

    for (int i = front; i <= rear; i++)
        printf("%c ", queue[i]);
}

int main()
{
    return 0;
}


```

## Output:
![image](https://github.com/user-attachments/assets/6b1348f5-936d-4b8f-9478-3a848914c08c)


## Result:
Thus the program was executed and the output was verified successfully.
