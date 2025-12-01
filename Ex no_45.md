
# EX 45 C program that implements a queue using an array, and performs insertion (enqueue) and display operations.
## DATE: 6.10.25
## AIM:
To write a C program that implements a queue using an array, and performs insertion (enqueue) and display operations. 

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a functions to traverse the linked list and display it in the following format. 
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
        printf("No elements to display");
        return;
    }

    for (int i = front; i <= rear; i++)
        printf("%c\n", queue[i]);
}

int main()
{
    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/b402ce73-b0c8-4b2c-9fe0-ddd383f0a3bb)



## Result:
Thus the program was executed and the output was verified successfully.
