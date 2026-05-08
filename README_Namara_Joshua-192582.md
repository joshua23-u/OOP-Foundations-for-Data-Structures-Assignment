# Assignment 1 (Namara Joshua-192582)

## Part 2: Basic OOP Practice — Node Class
I created a `Node` class with two attributes: `data` and `next`. 
I then manually created three nodes with values 10, 20, and 30, linked them together, and traversed the chain using a loop to print their values. This exercise helped me clearly understand how nodes connect to form a linked structure.

## Part 3: Simple Linked List
I implemented a `LinkedList` class that includes the three required methods: `append(data)`, `display()`, and `search(data)`. 
The code is clean, properly commented, and includes a demonstration section at the bottom to show the methods in action.

## Part 4: Conceptual Questions
### 1. What is the role of a class in a linked list?
A class acts as a blueprint for creating objects. In a linked list, we use two main classes. The `Node` class defines what each individual building block looks like by holding the data and the link to the next node. The `LinkedList` class manages the entire structure by keeping track of the head and providing methods to add, display, and search for data. Classes help us organize our code and bundle related data and behaviors together.

### 2. What is the difference between a node and a linked list?
A node is a single element that contains some data and a reference to the next node. On the other hand, a linked list is the complete collection made up of multiple nodes connected together. It has a head pointer and methods to perform operations like adding new nodes, searching, and displaying the list. 
In simple terms, a node is like one train car, while a linked list is the entire train.

### 3. Why do we use None in next?
We use `None` to mark the end of the linked list. It acts as a stop signal during traversal. When we go through the list, we keep moving to the `next` node until we reach `None`, which tells us there are no more nodes ahead. It also represents an empty list when the `head` is `None`. Using `None` helps prevent infinite loops and potential errors.

### 4. How is a linked list different from a Python list?
A linked list and Python’s built-in list are quite different in how they work under the hood. In a linked list, the nodes can be stored anywhere in memory and are connected to each other using pointers. This design makes inserting or deleting nodes at the beginning very fast, but accessing a specific element requires traversing the list from the head, which can be slow for large lists. In contrast, Python’s list is actually implemented as a dynamic array where all elements are stored in contiguous memory locations. This allows very fast access to any element by index, but inserting or removing elements at the beginning is slower because it requires shifting all the other elements. Overall, linked lists are better suited for situations where frequent insertions and deletions are needed, while Python lists are more efficient for random access and general-purpose use.

### 5. Why is OOP useful for data structures?
OOP is very useful for data structures because it allows us to create clean and organized code. We can hide the complex internal details (like pointer manipulation) behind simple methods. It promotes encapsulation by keeping the data and the operations that work on that data together in one class. This makes the code easier to understand, maintain, reuse, and extend later for other structures like stacks, queues, or trees.

## Files in This Repository
- `node.py` — Manual node creation and linking (Part 2)  
- `linked_list.py` — LinkedList class with required methods (Part 3)  
- `README_Namara_Joshua.md` — This file with explanations and answers
