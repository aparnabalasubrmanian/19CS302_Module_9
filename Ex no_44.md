
# EX 44 C functions to perform enqueue, dequeue, display, peek in Queue using Array.
## DATE: 6/10/2025
## AIM:
To write a C Write a functions to perform enqueue, dequeue, display, peek in Queue using Array.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a functions to perform enqueue,dequeue ,display,peek in Queue using array. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End   

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

float queue[100];
int front = -1, rear = -1;

void enqueue(float x)
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

void dequeue()
{
    if (front == -1)
    {
        printf("Queue Underflow\n");
        return;
    }

    if (front == rear)
    {
        front = rear = -1;
    }
    else
    {
        front++;
    }
}

void display()
{
    if (front == -1)
    {
        printf("no elements to display\n");
        return;
    }

    for (int i = front; i <= rear; i++)
        printf("%.1f\n", queue[i]);
}

void peek()
{
    if (front == -1)
    {
        printf("no elements to display\n");
        return;
    }

    printf("%.1f\n", queue[front]);
}

int main()
{
    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/3c69a98a-cbb9-4608-b259-f8cb31a3a653)


## Result:
Thus the program was executed and the output was verified successfully.
