- [What you should prepare?](#what-you-should-prepare)
  - [Big O](#big-o)
  - [Data Structures you should know](#data-structures-you-should-know)
  - [Fundamental algorithms you should know](#fundamental-algorithms-you-should-know)
- [Working with this repo](#working-with-this-repo)
- [Math & Stats](#math--stats)
  - [Integer Division Without Using \* or /](#integer-division-without-using--or-)
- [Mock Interview](#mock-interview)
  - [Get the Average value at each level of the tree](#get-the-average-value-at-each-level-of-the-tree)
  - [ADT](#adt)
- [Data-Structure](#data-structure)
  - [Array](#array)
    - [Implement Binary Search on a Sorted Array](#implement-binary-search-on-a-sorted-array)
    - [Find Maximum in Sliding Window](#find-maximum-in-sliding-window)
  - [Linked List](#linked-list)
    - [Insert at head](#insert-at-head)
    - [Insert at tail](#insert-at-tail)
    - [Reverse a Singly Linked List](#reverse-a-singly-linked-list)
  - [Stack](#stack)
  - [Queue](#queue)
  - [Tree](#tree)
    - [Binary Tree](#binary-tree)
    - [Binary Search Tree (BST)](#binary-search-tree-bst)
  - [Trie](#trie)
  - [Heap ( Priority Queue )](#heap--priority-queue-)
  - [Hash-Table](#hash-table)
  - [Graph](#graph)
  - [Graph Algorithms](#graph-algorithms)
    - [Depth-First Search (DFS)](#depth-first-search-dfs)
    - [Breadth-First Search (BFS)](#breadth-first-search-bfs)
    - [DFS Vs BFS](#dfs-vs-bfs)
- [Sorting](#sorting)
  - [Merge Sort](#merge-sort)
- [Math.floor](#mathfloor)
- [Math.round](#mathround)

### What you should know before coding interview?

Make sure you know Computer science [basic data structures](#data-structures-you-should-know). Also you should be aware of [fundamental algorithms](#fundamental-algorithms-you-should-know).

### Ask Questions before coding

Once they give you problem, don't start coding. Ask clarifying questions to make sure you understand the problem.

Example:

- Will there be null/empty values on input?
- Will all numbers in a binary tree integers?
-

## What you should prepare?

### Big O

Learn Big O. Make sure you give what would be the `runtime complexity` and `memory complexity`.

`Iterative functions` take no extra memory and therefore, `memory complexity` is `constant` O(1).

`Recursive functions` take extra on the stack therefore, `memory complexity` is `lograrithmic` O(_logn_)

### Data Structures you should know

- Hash Table
- Linked List
- Stack
- Queue
- Tree
- Tries
- Graphs
- Vectors
- Heaps

### Fundamental algorithms you should know

- Breadth-first search
- Depth-first search
- Merge sort & Quick sort

## Working with this repo

Download or clone in local machine. Then run individual file in node console to see the results.

## Math & Stats

### Integer Division Without Using \* or /

Divide two integers without using '/' (division) or '\*' (multiplication) operators.

```shell
node .\src\math-and-stats\integer-division.js
```

![](https://imgur.com/Cf7cz4W.png)

## Mock Interview

### Get the Average value at each level of the tree

![](https://imgur.com/N6agnSk.png)

Traverse by depth and collect all the numbers.
And calculate average also.

Runtime Complexity
O(logn)
Space Complexity
O(logn)

### ADT

abstract data type (ADT) - ADT is defined as a user point of view of a data type and Does not talk about how exactly it will be implemented.

## Data-Structure

Data-structure represents how data will be stored in memory.

### Array

Arrays can store a fixed number of elements, whereas a collection stores object dynamically so there is no size restrictions it grows and shrinks automatically.

- **Insert** at the end (push) is efficient.

#### Implement Binary Search on a Sorted Array

Given a sorted array of integers, return the index of the given key. Return -1 if the key is not found.

Run below script

```
node .\src\arrays\binary-search.js
```

#### Find Maximum in Sliding Window

Given a large array of integers and a window of size w, find the current maximum value in the window as the window slides through the entire array.

### Linked List

Linked lists are dynamic data structure and memory is allocated at run time. They don't store data contiguously rather they use link to point to other elements.

![](https://i.imgur.com/tMN6TD5.png)

Performance wise linked lists are slower than arrays because there is no direct access to linked list elements.

Suppose we have an array that contains following five elements 1, 2, 4, 5, 6. We want to insert a new element with value “3” in between “2” and “4”.

You have to copy 1,2 in new array then insert 3 and copy rest of the values. Runtime complexity and memory complexity is very high.

Therefore, we use linked list to store 1-6 and we can easily insert 3 in between 2 and 4.

![](https://i.imgur.com/r689svn.png)

The linked list is a list of items, called nodes. Nodes have two parts, `value` part and `link` part. Value part is used to stores the data. The link part is a reference, which is used to store addresses of the next element in the list.

- **Head**: Head is a reference that holds the address of the first node in the linked list.
- **Nodes**: Items in the linked list are called nodes.
- **Value**: The data that is stored in each node of the linked list.
- **Link**: Link part of the node is used to store the reference of other node.

![](https://i.imgur.com/LeGU67n.png)

![](https://i.imgur.com/nHFfpov.png)

```ts
class LinkedListNode {
  constructor(data) {
    this.data = data;
    this.next = null;
  }
}
```

Below are the types of LinkedList:

- **Singly Linked List**
- **Doubly Linked List**
- **Circular Linked List**

  ![](https://i.imgur.com/byjRY7x.png)

#### Insert at head

The newly created node will become head of the linked list. · Size of the list is increased by one.

![](https://i.imgur.com/79qwSqL.png)

#### Insert at tail

![](https://i.imgur.com/Wz9Uovq.png)

#### Reverse a Singly Linked List

We’re given the pointer/reference to the head of a singly linked list, reverse it and return the pointer/reference to the head of the reversed linked list.

![](https://i.imgur.com/lamsYrL.png)

Problem Solving steps

![](https://i.imgur.com/0wZ4lB1.png)

Running program output

![](https://i.imgur.com/FAHJMeF.png)

### Stack

Depth First Search (DFS) uses a `stack` for storing the nodes that it is visiting.

### Queue

Breadth First Search (BFS) uses a `queue` for storing the nodes that it is visiting.

### Tree

A tree has hierarchical data and it has nodes.

![](https://i.imgur.com/wUiUy0B.png)

- **Root**: top node of tree is called root and has no parent and has no incoming edges.
- **Node**: every node has parent ( except root ) and 0 or more children's.
- **Edge**: used to connect two nodes.
- **Path**: A path is an ordered list of nodes that are connected by edges.
- **Leaf**: A leaf node is a node that has no children.
- **Height of the tree**: The height of a tree is the number of edges on the longest path between the root and a leaf.
- **The level of node**: The level of a node is the number of edges on the path from the root node to that node.
- **Children**: Nodes that have incoming edges from the same node to be said to be the children of that node.
- **Parent**: Node is a parent of all the child nodes that are linked by outgoing edges. - **Sibling**: Nodes in the tree that are children of the same parent are called siblings.
- **Ancestor**:  A node reachable by repeated moving from child to parent.

![](https://imgur.com/L04E7lo.png)

![](https://i.imgur.com/Jzwpguk.png)

If you want to store hierarchical data use Tree.

You should know about `Binary Tree` and `Binary Search Tree`.

#### Binary Tree

A binary tree is a type of tree in which each node has `at most two children` (0, 1 or 2) which are referred as left child and right child.

![](https://i.imgur.com/fkRP5Ju.png)

#### Binary Search Tree (BST)

In Binary Search Tree nodes are:

- The key in the left subtree is less than the key in its parent node.
- The key in the right subtree is greater or equal the key in its parent node.

![](https://i.imgur.com/Dk04fw4.png)

### Trie

Trie is a tree, in which we store only one character at each node. This final key value pair is stored in the leaves.

![](https://i.imgur.com/o9UWgEN.png)

Trie is also suitable for solving partial match and range query problems.

### Heap ( Priority Queue )

Each node in the heap follows the rule that the `parent value is greater than its two children` are.

![](https://i.imgur.com/J5If65C.png)

There are two types of the heap data structure:

- **Max heap**: each node should be greater than or equal to each of its children.
- **Min heap**: each node should be smaller than or equal to each of its children.

A heap is a useful data structure when you want to get max/min one by one from data.

### Hash-Table

It is just like a dictionary or key value pair.

### Graph

![](https://i.imgur.com/kYlxMWJ.png)

Graph represents network. It has Nodes, Vertices and Edges.

### Graph Algorithms

- Depth-First Search (DFS)
- Breadth-First Search (BFS)

#### Depth-First Search (DFS)

The DFS algorithm we start from starting point and go into depth of graph until we reach a dead end and then move up to parent node (Backtrack). The stack is used to implement DFS.
![](https://i.imgur.com/4P7FMDl.png)

#### Breadth-First Search (BFS)

In BFS algorithm, a graph is traversed in layer-by-layer fashion. point. The queue is used to implement BFS.

![](https://i.imgur.com/i7nf4go.png)

Example: Suppose you have given a tree structure and asked to calculate the average of numbers at each level.

#### DFS Vs BFS

| DFS                                                                       | BFS                                                                                                      |
| ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Search from root to the leaf                                              | Search level by level                                                                                    |
| Uses Stack to sort                                                        | Uses Queue to sort                                                                                       |
| Time complexity: Fast                                                     | Time complexity: Slow                                                                                    |
| Where to use: if you can find at root or leaf, find connected components. | Where to use: Find shortest path,find connected components. When you think you have less data go for it. |


## Sorting 

### Merge Sort

Browser's JavaScript Engine (`Array.prototype.sort`) uses merge sort maximum time. Runtime complexity O(n logn), Memory complexity O(n) because we have to create new list. It uses divide-and-conquer algorithm! and also it is recursive.


## Math.floor 
2.5 = 2
2.8 = 2
2.4 = 2

## Math.round
2.5 = 3
2.8 = 3
2.4 = 2