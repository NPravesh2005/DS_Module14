# Ex6 Dequeue Elements from Circular Queue
## AIM:
To write a C program to delete three elements from the filled circular queue.

## Algorithm
1. Start and initialize a fixed-size queue with front = rear = -1.
2. In deQueue(), check if queue is empty using isEmpty().
3. If empty, display error; if one element, reset front and rear to -1.
4. Otherwise, update front = (front + 1) % SIZE.
5. Return the removed element and end.

## Program:
```c
/*
Program to delete three elements from the filled circular queue
Developed by: PRAVESH N
RegisterNumber:  212223230154
*/
/*#include<stdio.h>
#define SIZE 5
int items[SIZE];
int front =-1,rear =-1;
*/
int deQueue()
{
int element;
element=items[front];
if(isEmpty())
{
printf("Queue isEmpty!!");
}
else
{
if(front==rear)
{
front=-1;
rear=-1;
}
else
{
front=(front+1)%SIZE;
}
}
return element;
}

```

## Output:

![image](https://github.com/user-attachments/assets/23cd2dff-a7b8-4874-9827-f8393f744757)


## Result:
Thus, the C program to delete three elements from the filled circular queue is implemented successfully.
