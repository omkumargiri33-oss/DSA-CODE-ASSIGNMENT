# 1st.-Linear-Queue
Operations: Insert 10, 20, 30 → Delete 2 → Insert 40 → Display

#include <stdio.h>

#define MAX 5

int queue[MAX];
int front = -1, rear = -1;

void insert(int value)
{
    if (rear == MAX - 1)
    {
        printf("Queue Overflow\n");
    }
    else
    {
        if (front == -1)
            front = 0;

        rear++;
        queue[rear] = value;
    }
}

void delete()
{
    if (front == -1 || front > rear)
    {
        printf("Queue Underflow\n");
    }
    else
    {
        printf("Deleted: %d\n", queue[front]);
        front++;
    }
}

void display()
{
    int i;

    if (front == -1 || front > rear)
    {
        printf("Queue is empty\n");
    }
    else
    {
        printf("Remaining elements: ");

        for (i = front; i <= rear; i++)
        {
            printf("%d ", queue[i]);
        }

        printf("\n");
    }
}

int main()
{
    insert(10);
    insert(20);
    insert(30);

    delete();
    delete();

    insert(40);

    display();

    return 0;
}
