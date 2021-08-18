# Linked Lists


## Linked Lists

### What does it look like?
![linkedlist](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

- linked list is a collection of nodes, starting with head object that will be null when the linked list is empty, then when adding the first node will update the value of the head to this node object, including the next propert that will point to the reference of the next node if it exist or null if it was the last node in the linked list.


> - if we add a node to the first BigO of time will be O(1), but if we add between nodes or at the end, BigO of time will be O(n). and in the both cases the BigO of space will be as the value of nodes, and mostly will be O(1).

> - there are two types of linked lists : singly & doubly; the difference is the singly only have one pointer to the next node. but the doubly has two pointers; the first one for the next node and the second one for the previous node.

### data structures 

> In computer science, a linked list is a linear collection of data elements whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of nodes which together represent a sequence. 


> Linked List is a very commonly used linear data structure which consists of group of nodes in a sequence. Each node holds its own data and the address of the next node hence forming a chain like structure. Linked Lists are used to create trees and graphs

![](https://cdn-media-1.freecodecamp.org/images/VSLri8VM6VeXUN4Ml43JlFh6SspOdtkXNkj-)


### Memory management

![Memory management](https://miro.medium.com/max/700/1*G43FVT5xJ1n1QDKVNZUxXQ.jpeg)



## Linked List?
- O(1) : means i need a constant time & and same space, and doesn't matter how much the elements we have or how huge our input is.
- O(n) : means that as our input grows, the space and time that we need to run that algorithm grows linearly.
- a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.
 data structures : ways of organizing our data.
- linked lists are a linear data structure, that means we traversed over the data sequentially.
- arrays and linked lists are linear data structure.


### How structure is used in linked list?
1. Insert node at the beginning.
2. Insert node in the middle
3. Insert node at the end

### Example of Linked List !!
![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2014/03/DLL1.png)


### a diagram
![](https://i.ytimg.com/vi/pBrz9HmjFOs/maxresdefault.jpg)

### a map 
![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20190621160855/Detect-loop-in-a-linked-list.png)