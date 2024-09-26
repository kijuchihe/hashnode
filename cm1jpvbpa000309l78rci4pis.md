---
title: "Arrays in DSA"
seoTitle: "Arrays in Data Structures and Algorithms"
seoDescription: "An array is an ordered data collection. Learn about types, operations, uses, advantages, and disadvantages of arrays in data structures"
datePublished: Thu Sep 26 2024 19:58:21 GMT+0000 (Coordinated Universal Time)
cuid: cm1jpvbpa000309l78rci4pis
slug: arrays-in-dsa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1727380586893/f2ffb63d-bab1-4b3d-b3fa-c893cfe51004.jpeg
tags: algorithms, data-structures, array, dsa

---

## What is an Array?

An array is an ordered collection of data (usually of the same data type). However, recent languages allow for arrays of multiple data types.

Elements are allocated contiguous memory, allowing for constant-time access. Each element has a unique identification number called its `index`.

Now enough of these complex terms😅.

Picture your **kitchen cupboard** where you store all your essential items. To keep things tidy and easy to find, you decide to organize your cupboard by grouping similar items together and giving each item in a unique number in that group. This organized collection is like an **array**—a way to hold multiple items in one place.

## Types of Arrays

Arrays can generally be classified into two types:

1. One-dimensional arrays
    
2. Multi-dimensional arrays
    

## Operations on an Array

1. Insertion
    
2. Reading (Searching)
    
3. Traversal
    
4. Deletion
    

### Insertion into an Array

Arrays store elements in a contiguous block of memory. This means that: elements are next to each other in the array and all occupy one whole block of memory.

To insert a new item to the end of the array, you’ll have to first of all go through the array starting from the first item then when you get to the last item, you append the new item to the array.

> Insertion at the end has a time complexity of O(n).

To add a new item to the beginning of the array, you’ll have to first of all shift all the elements to the right (the following block of memory), then you add the new item at the beginning.

> Adding a new item at the beginning also has a time complexity of O(n).

### Reading an element

We have established the fact that each element in an array has an index (zero-based index). For this reason, reading an item is much easier. Once we know the index (`i`), we just do some basic math to get the item at that index.

```plaintext
Memory address of array + (i * size of data type being stored)
```

> Reading an element has a time complexity of O(1)

### Delete an item

To delete a certain item, you’ll have to first of all go through the array till you get to the one you want to delete. This operation is proportional to the number of items in the array.

> The time complexity of deletion in an array is O(n)

## Uses of Arrays

Arrays have multiple uses of which I will list a few.

* Storing data in a sequential manner
    
* Implementing queues, stacks, and other data structures
    
* Representing matrices and tables (Uses of 2d-arrays).
    

## Advantages of using an array

1. **Organization**: Just like your cupboard helps you keep track of what you have, an array organizes information so you can find it easily.
    
2. **Easy Access**: When you want to set the table, you can quickly see all your plates, cups, and cutlery without rummaging through everything.
    
3. **Flexibility**: If you buy new items, like a set of **serving trays**, you can easily add them to your cupboard!
    

## Disadvantages of using an array.

1. Unused memory: generally, when you define an array, you give it a specific amount of memory to take up. This amount of memory is usually large in case we want to add extra items to the array. However, a lot of times we may not store up to the amount that was set causing the wastage of memory that has been allocated to it.
    
2. Dynamic Arrays: in the case where we actually use up the memory but we need more, how do we go about it? Well, that is where dynamic arrays come in. To implement a dynamic array, we will allocate a new block of memory that is twice the original size and then move all the items from the old one to the new one and then add the new item. Already reading that, it sounds like a lot of time and space being wasted😂😅. The first time I saw it, I said to myself: what happens to the rest of the space that was created😂🤷🏾‍♂️.
    
3. Creating dynamic arrays as seen above is very time costly. That has a time complexity of `O(n)`.
    

### Conclusion

Just like your well-organized kitchen cupboard makes cooking and serving meals easier, an array helps keep information structured and accessible in various situations. It’s all about making life simpler and more enjoyable.

That still doesn’t mean it doesn’t come with its own disadvantages.