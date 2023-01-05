7 JavaScript Data Structures you must know
#
javascript
#
webdev
#
programming
#
datastructures
Data Structures is one of the most frequently tested subjects by a lot of companies. It is the base of IT industries and is largely used in the areas of Artificial Intelligence, operating systems, graphics, etc.
In this blog post, I will cover the seven most used JavaScript data structures that every JS developer should know.

This Blog Post will cover:-
- What are Data Structures?
- 7 most used data structures
  - Arrays
  - Stack
  - Queues
  - Linked List
  - Trees
  - Graphs
  - Hashtable
What is Data Structures?
Data Structure is the way of storing and organizing the data in such a way that it can be used efficiently. More precisely, Data Structure refers to a group of data values, how they relate to each other, and the operations or functions that can be carried out on them.

Data structures= group of data values+allowed operations on that data.

Data structure enables us to manage and utilize large datasets, handle multiple requests from users at once, and speed up the data processing.

Types of data structures in JS:-
Screenshot (210).png

1.) Array
Arrays are the most basic data structure. It is a group of similar types of elements stored together at contiguous memory locations and each cell has a corresponding numeric index used to select its data. Like all scripting languages​​, JavaScript has dynamic arrays i.e their size is not predetermined, nor the type of data.

An array literal is the easiest way to create a JavaScript Array.
Let's see the simple example of creating an array using an array literal:-
<script>  
var users=["neha","ayushi","gauri"];  // creating an array
//iterate over an array 
for (i=0;i<users.length;i++){  
document.write(users[i] + ", ");  
}  
</script>  
Output:- neha, ayushi, gauri

Common JavaScript Array Methods:-
ArrayMethods

Linked List
The linked list is a linear data structure in which elements are not in contiguous memory locations. It consists of a group of nodes and each node has its own data and address to the next node. In an array, the elements are indexed and you can instantly get to an element but in a linked list, you have to start with the head and work your way through until you get to the desired element. The advantage of the linked list is that the insertion and deletion in linked list are easier than array, as the elements in an array are stored in a consecutive location. Also, its memory consumption is efficient as the size of the linked list can grow or shrink according to our requirements.
Screenshot (216).png

Basic Operations on Linked List
Screenshot (218).png
Check the implementation of the linked list in JS here

Stack
Stack is a linear data structure that follows the LIFO(Last In First Out) or FILO(First In Last Out) principle. It contains only one pointer the top pointer that points to the topmost element of the stack. Whenever we add an element to the stack, it is added at the top of the stack and also whenever we delete an element from the stack it is deleted from the top of the stack.
stack exaamples.jpg

Common operations implemented on the stack:-
Screenshot (207).png
Check the implementation of stack in JS here.

Queues
Queue is a linear data structure that follows the FIFO(First In First Out) principle. It contains two-pointers, 1) front pointer, 2) rear pointer. The front pointer contains the address of the starting element and the rear pointer contains the address of the last element of the queue. The two main methods used for the implementation of the queue are the enqueue and dequeue method. Enqueuing is the process of adding an element in the queue and dequeuing is the process of removing an element from the queue.

queue example.png

Basic operations:-
A queue is an object that allows the following operations-

Screenshot (212).png
Check the implementation of queue in JS here.

Trees
The tree is a non-linear hierarchical data structure consists of nodes connected by edges. Each node contains some data and the link of other nodes that can be called children. The topmost node of the tree is known as a root node. Nodes with linked child nodes are called internal nodes while those without child nodes are external nodes(leaf nodes).
There are a number of different types of trees:-

1.) Binary Tree
2.) Binary Search Tree
3.) AVL Tree
4.) Balanced tree
5.) Red black tree
6.) 2-3 tree
7.) N-ary tree

Binary Tree and Binary Search Tree are typically the most often used.

Tree Representation:-
Screenshot (224).png

Basic Terminology
Node => A node is an entity that contains a data and pointer to its child nodes.
Edge => The connecting link between any two nodes is called as Edge.
Root => It is the topmost node of a tree.
Parent => The node which is a predecessor of any node is called as Parent Node.
Child => The node which is a descendant of any node is called as Child Node.
Siblings => Nodes that belong to the same parent are called Siblings.
Leaf => The node which does not have a child is called Leaf Node.
Internal Nodes => The node which has atleast one child is called Internal Node.
Degree => The total number of children of a node is called as DEGREE of that Node.
Level => Each step from top to bottom is called the Level of a tree. The root node is said to be at Level 0 and the children of the root node are at Level 1 and the children of the nodes which are at Level 1 will be at Level 2 and so on...
Height of a Node => The Height of a Node is the number of edges from the node to the deepest leaf (ie. the longest path from the node to a leaf node).
Height of a Tree => The Height of a Tree is the height of the root node or the depth of the deepest node.
Depth of a Node => The Depth of a Node is the number of edges from the root to the node.
Depth of a Tree => The Depth of a Tree is the total number of edges from the root node to a leaf node in the longest path.
Check the implementation of tree in JS here.

Graphs
A graph is a common data structure consists of a finite set of nodes and edges. A graph can be seen more like a network. The interconnected objects are represented by points known as vertices, and the links that connect the vertices are called edges. A vertex is just similar to the linked list nodes and the pair (x,y) referred as an edge which means that the x vertex connects to the y vertex. The graphs can be represented using an adjacency matrix or adjacency list.

Graphs are the ultimate abstraction for many real-world problems. Some of the best use cases for Graph Data Structures include Social Graph APIs(like LinkedIn, Facebook, etc.), Path Optimization Algorithms(like Google maps), Web Analytics and Scientific Computations.

There are two common types of graphs:-

Undirected Graphs => In an undirected graph, edges are not associated with the directions with them. It means if an edge exists between vertex X and Y then the vertices can be traversed from Y to X as well as X to Y.
Directed Graphs => In a directed graph, edges are associated with the directions with them. It means if an edge exists between vertex X and Y then the vertices can be traversed from X to Y only. Here, vertex A is called the initial node while vertex B is called the terminal node.
Screenshot (226).png

Basic Terminology
Path => Path represents a sequence of edges between the two vertices.
Simple Path => A simple path is a path in which all the nodes of the graph are distinct with an exception0=VN.
Closed Path => A simple path is a path in which the initial node is same as a terminal node.
Cycle => A cycle can be defined as the path which has no repeated edges or vertices except the first and last vertices.
Complete Graph => A graph in which every vertex is directly connected to all other vertices.
Connected Graph => A Connected graph has a path between every pair of vertices
Weighted Graph => A weighted graph associates a value (weight) with every edge in the graph.
Loop => An edge that is associated with similar endpoints can be called a Loop.
Degree => The degree of a vertex in a graph is the total number of edges incident to it.
Adjacent Nodes(vertices) => Two vertices are called adjacent if they are connected via same edge.
Basic Operations on Graph
Screenshot (228).png
Check the implementation of graph in JS here.

Hash Tables
Hash Table(also called a hash, hash map) is a data structure that stores the data in an associative manner using hashing. Hashing is the technique of mapping keys, values into the hash table by using a hash function. Here “key” is a searched string and the “value” is the data paired with that key. By using a good hash function, hashing can work well. In the hash table, the insertion and search operations are very fast irrespective of the size of the data. Hash tables are built using arrays.

Screenshot (230).png
Real-life examples of the hash table:-

In school/universities, each student is assigned a unique roll number that can be used to retrieve information about them.
In libraries, each book is assigned a unique number that can be used to determine information about the book,
Basic Operations
Insert:- inserts an element in a hash table.

Delete:- Deletes an element from a hash table.

Search:- Searches an element in a hash table.

Check the implementation of hash tables in JS here

Final Thoughts on Data Structures
For many developers and programmers, data structures are most important for cracking Javascript coding interviews. Each data structure has a number of different applications and uses. So, having a basic understanding of data structures is a critical first step to becoming a good programmer.

In this blog, we have just scratched the surface of data structures in JavaScript. If you enjoyed learning and find it useful please do like and share so that, it reaches others as well 🤝