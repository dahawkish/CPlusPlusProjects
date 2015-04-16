How to put elements into a queue, and how to implement the First in First Out idea?

There are some templates from the textbooks, and here is my version. 

There are several things we need to pay attention about a queue:

1. Full queues and empty queues;
2. enqueue -ing adds front the back enqueue(queue, 10);
3. dequeue -ing behaves like dequeue(queue);

Creating a queue using linked list:

struct Queue *createQueue(unsigned capacity)
{
    struct Queue *queue = (struct Queue*) malloc(sizeof(struct Queue));
    queue->maximumLength = maximumLength;
    queue->front = queue->currentSize = 0;
    queue->rear = maximumLength - 1;  
    queue->array = (int*) malloc(queue->capacity * sizeof(int));
    return queue;
}

There are other ways to create the queue...see BFS_graph and DFS_graph
