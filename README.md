## Data Structures
- Data structures are an integral part of computers used for the arrangement of data in memory. 
- They are essential and responsible for organizing, processing, accessing, and storing data efficiently. 
- But this is not all. Various types of data structures have their own characteristics, features, applications, advantages, and disadvantages.
- So how do you identify a data structure that is suitable for a particular task? What is meant by the term ‘Data Structure’? 
- How many types of data structures are there and what are they used for?

![image](https://user-images.githubusercontent.com/105867034/178478615-f45c9c89-b567-426a-b291-82235248132f.png)

### Types of Data Structures
- Arrays: An array is a collection of elements of the same type placed in contiguous memory locations.
- Linked Lists: It is a linear data structure, in which the elements are not stored at contiguous memory locations and the elements are linked with each other.
- Stacks: Follow LIFO (Last In First Out) principle. In this, the last element in the stack will be removed first.
- Queues: It follows the FIFO principle (First In First Out), in this, the first element stored is removed first.
- Hash Tables: This is a type of data structure that stores values which have keys related to each of them.
    + Ultimate Objectives of Hashing
        + Minimize Collision
        + Minimize Overflow
        + Minimize Hash Table Size: Keep N(indexes) and/or K(buckets) reasonably small
    + Commonly Used Hash Functions
        + Modulo(Division) Function
        + Digit Folding("hashing")
        + Digit Selection
        + Mid-Square Function

- Trees: It is a data structure in which data is organized hierarchically and linked together. Some Examples are the Binary Search tree, Binary tree, Splay tree, AVL Tree, etc.
    + Differences between B-Tree and T-Tree
        + T-Tree
            + a main-memory data structure
            + a binary tree
            + height-balanced, but not perfectly
            + rebalancing uses tree rotations
        + B-Tree(and B+) Tree
            + an external data structure
            + an m-way tree
            + perfectly height-balanced
            + rebalancing uses node split and merge
            * B-Tree
                * Tree height is taller, because each node can contain fewer keys
                * Has no support for range queries
                * Search may end before reaching the leaf level
            * B+ Tree
                * Tree height is smaller, because each node can contain more keys
                * Has support for range queries
                * Search must continue to the leaf level

    + Degree of Trees
        + Unary Tree: linked list
        + Binary Tree: binary search tree
        + m-way Tree(m>2)
    + Height Balance
        + Unbalanced
        + Balanced (but not perfectly): AVL tree, T-tree
        + Perfectly Balanced: 2-3 tree
    + Dimension
        + One Dimension: AVL tree, T-tree
        + n-dimention(n>=2): quad tree, kd tree
    
- Heaps: It is a specialized tree-based data structure, also called binary heap in which data is stored.
- Graphs: It consists of a set of nodes and edges connecting each other.
    + Topics
        + Graph Representaion: Adjacency Matrix/Lists
        + Graph Traversal: DFS, BFS
        + Spanning Tree: A Tree of N Nodes and N-1 edges, Cycles are removed from the graph
        + Minimum Spanning Tree: A spanning tree with a minimum total weight of all the edges
        + Minimum Spanning Tree Algorithm
            + Prim's algorithm / Kruskal's algorithm / Dijkstra's algorithm / Warshall's algorithm
        + Transitive Closure Algorithms

## Algorithm
<img src=https://user-images.githubusercontent.com/105867034/178479808-21ab10ae-2842-4e71-8f65-8e64fee8a340.png width=600px height=350px></img>

### Characteristics of Algorithm
- Clear and Unambiguous: The algorithm should be clear and unambiguous. Each of its steps should be clear in all aspects and must lead to only one meaning.
- Well-Defined Inputs: If an algorithm says to take inputs, it should be well-defined inputs. 
- Well-Defined Outputs: The algorithm must clearly define what output will be yielded and it should be well-defined as well. 
- Finite-ness: The algorithm must be finite, i.e. it should terminate after a finite time.
- Feasible: The algorithm must be simple, generic, and practical, such that it can be executed with the available resources. It must not contain some future technology or anything.
- Language Independent: The Algorithm designed must be language-independent, i.e. it must be just plain instructions that can be implemented in any language, and yet the output will be the same, as expected.

### Types of Algorithm
1. Brute Force Algorithm             
2. Recursive Algorithm        
3. Backtracking Algorithm         
4. Searching Algorithm         
5. Sorting Algorithm         
6. Hashing Algorithm         
7. Divide and Conquer Algorithm          
8. Greedy Algorithm        
9. Dynamic Programming Algorithm         
10. Randomized Algorithm           

* DP - Tabulation vs Memoization
![image](https://user-images.githubusercontent.com/105867034/179345150-4a659eb6-657d-4543-97d9-13b16ffe2c58.png)

* Graph Algorithm
1. Prim / Kruskal / Dijkstra / Bellman-Ford algorithm -> Greedy Algorithm (Single-Source Shortest Paths)
2. Floyd-Warshall algorithm (Using matrix multiplication) -> Dynamic Programming (All-Pairs Shortest Paths)

### Analysis of Algorithms
#### Asymptotic Analysis
Asymptotic Analysis is the big idea that handles above issues in analyzing algorithms. In Asymptotic Analysis, we evaluate the performance of an algorithm in terms of input size (we don’t measure the actual running time). We calculate, how the time (or space) taken by an algorithm increases with the input size.
- Notations: Theta / Big O / Omega

#### Worst, Average and Best Cases
- Best case : Order of growth will be constant because in the best case we are assuming that (n) is even
- Average case : In this case we will assume that even and odd are equally likely, therefore Order of growth will be linear
- Worst case : Order of growth will be linear because in this case we are assuming that (n) is always odd

#### Analysis of Loops
![image](https://user-images.githubusercontent.com/105867034/178682126-ee262e93-a431-4587-9a08-4a2ae0c40b15.png)

#### Solving Recurrences
1. Substitution Method
2. Recurrence Tree Method
3. Master Method
    - T(n) = aT(n/b) + f(n) where a >= 1 and b > 1
    ![image](https://user-images.githubusercontent.com/105867034/178762463-84b67a44-a09c-4d01-bbfb-b45c39d0fe4d.png)
    ![image](https://user-images.githubusercontent.com/105867034/178763114-e74d2ad5-7b40-455d-96aa-8c63edea5f68.png)

## P-NP Problem
The P versus NP problem is a major unsolved problem in theoretical computer science. In informal terms, it asks whether every problem whose solution can be quickly verified can also be quickly solved.
The problem has been called the most important open problem in computer science. Aside from being an important problem in computational theory, a proof either way would have profound implications for mathematics, cryptography, algorithm research, artificial intelligence, game theory, multimedia processing, philosophy, economics and many other fields.

NP-complete problems are a set of problems to each of which any other NP-problem can be reduced in polynomial time and whose solution may still be verified in polynomial time.

![image](https://user-images.githubusercontent.com/105867034/180583274-adb21f60-60c4-4479-b844-c97c95832417.png)


