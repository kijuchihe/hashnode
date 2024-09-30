---
title: "Queues and Stacks in DSA"
seoTitle: "Stacks and Queues in Data Structures and Algorithms"
seoDescription: "An overview of queues and stacks in data structures, their operations, types, applications, and importance in computer science"
datePublished: Mon Sep 30 2024 21:11:10 GMT+0000 (Coordinated Universal Time)
cuid: cm1pi8dnk000y0al7fivp3qks
slug: queues-and-stacks-in-dsa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1727730506444/a821f105-4538-436b-9f97-98638d5c7225.jpeg
tags: software-development, queue, stacks, dsa

---

## What are Queues?

A **queue** in data structures is a linear data structure that operates on the **First In First Out (FIFO)** principle. This means that the first element added to the queue will be the first one to be removed, similar to people lining up for a bus—whoever arrives first gets on first \[not in my country though :) \].

### Structure of a Queue

There are two points that we generally care about in a queue:

* **Front**: Points to the first element.
    
* **Rear**: Points to the last element.
    

In a queue, you can access both the first and the last items of the queue.

### Operations on a Queue

* **Enqueue**: This is the process of adding an item to a queue. This has a time complexity of `O(1)`
    
* **Dequeue**: This is the process of removing an item from a queue. This also has a time complexity of `O(1)`
    
* **Front**: This means seeing the first item of the queue `O(1)`
    

### Types Of Queues

1. **Simple Queue**:
    
    * The most basic type where elements are added at the rear and removed from the front.
        
    * Strictly follows FIFO.
        
2. **Circular Queue**:
    
    * Similar to a simple queue, but the last element connects back to the first, forming a circle.
        
    * This structure improves memory utilisation by allowing the reuse of empty spaces.
        
3. **Priority Queue**:
    
    * Each element has a priority level; elements are removed based on priority rather than order.
        
    * Useful in scenarios where certain tasks need to be processed before others, like CPU scheduling.
        
4. **Deque (Double-Ended Queue)**:
    
    * Allows insertion and removal of elements from both the front and rear.
        
    * Provides more flexibility compared to standard queues.
        

### Applications of Queues

Queues are widely used in various applications, such as:

1. Managing tasks in CPU scheduling.
    
2. Handling print jobs in printers.
    
3. Organising requests in web servers.
    

Queues are essential for maintaining order and ensuring fair processing of tasks, making them a fundamental concept in computer science.

## Stacks

A **stack** is a linear data structure that follows the **Last In First Out (LIFO)** principle. This means that the last element added to the stack is the first one to be removed. You can think of it like a stack of plates—only the top plate is accessible at any time \[except it is my Mom taking a plate from the stack and she drags it out\].

### Structure of Stacks

Stacks operate from one end, known as the **top**, where all operations are performed.

### Operations performed on tasks.

1. **Push()**: Adds an element to the top of the stack. This has a time complexity of `O(1)`.
    
2. **Pop()**: Removes the top element from the stack. This has a time complexity of `O(1)`.
    
3. **Peek() / Top()**: Returns the top element without removing it. This has a time complexity of `O(1)`.
    
4. **isEmpty()**: Checks if the stack is empty; returns true if it is. This has a time complexity of `O(1)`.
    
5. **isFull()**: Checks if the stack has reached its maximum capacity; returns true if it is full. This has a time complexity of `O(1)`.
    
6. **size()**: Returns the number of elements currently in the stack. This has a time complexity of `O(1)`.
    

### Applications of Stacks

1. **Function Call Management**:
    
    * Stacks are used to manage function calls in programming languages. Each function call creates a stack frame, allowing for nested calls and maintaining the execution context.
        
2. **Expression Evaluation**:
    
    * Stacks help evaluate arithmetic expressions, especially in converting infix expressions to postfix (Reverse Polish Notation) and evaluating them.
        
3. **Undo/Redo Functionality**:
    
    * Many applications, like text editors and graphic design software, use stacks to implement undo and redo features, allowing users to revert or redo actions easily.
        
4. **Backtracking Algorithms**:
    
    * Stacks are essential in algorithms that require backtracking, such as solving mazes or puzzles (e.g., depth-first search).
        
5. **Memory Management**:
    
    * In programming, stacks manage memory allocation for local variables and function calls, making it easier to allocate and deallocate memory dynamically.
        
6. **Browser Navigation**:
    
    * Web browsers use stacks to maintain the history of pages visited, allowing users to go back and forth through their browsing history.
        
7. **Plate and Coin Stacking**:
    
    * Real-world examples include physical stacks, such as plates on a tray or coins stacked on top of each other.
        

## Conclusion

So there you have it! Stacks and queues are essential tools for organizing data. Stacks let you work with the last item added first, while queues keep everything in order from first to last. Whether you're coding or just waiting in line at your favourite spot, understanding these structures can make things way easier.

In my next article, I’ll dive into **hashmaps**, exploring how they work and their applications. Following that, we’ll look into the implementations of the data structures we've discussed so far in multiple programming languages like \[C, python, typescript - depending on the one I choose ;-)\], along with some key algorithms that utilise them. Stay tuned for more insights into the fascinating world of data structures!