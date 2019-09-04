# Time Complexities
* Constant Time [ O(1) ]
* Sublinear Time [ O(log N) ]
* Linear Time [ O(N) ]
* SuperLinear Time [ O(N log N) ]
* Polynomial Time [ O(N ^ 2) ]
* Exponential Time [ O(K ^ N) ]
* Factorial Time [ O( N! ) ]

---
## 1. Constant Time
> when the algorithm deals with Simple Assignment. Only single step!

Time Complexities: [ O(1) ]

examples:
1. A *return* statement 
2. Accessing element with array index
3. pushing / popping in a stack
4. Insertion/Deletion in a queue
5. Inserting a node in a tree

> Efficient ? *Yes* !

## 2. Sublinear Time 
> The algorithms which get terminated in the middle-ish of its process

Time Complexity: [ O(log N) ]

examples: 
1. binary search
2. Searching and Element in Binary Search Tree
3. If then else if ladder

> Efficient ? *Yes* ! 

## 3. Linear Time
> Bruteforce Algorithms and Noob code written with for loops 

Time Complexitie: [ O(N) ]

examples:
1. Traversing an array: finding length of an array in "C Language"
2. Finding Smallest/ Largest element in a BST (Since small element is on the leaf nodes)
3. for loops are a good example.
4. Checking for palindromes.

> Efficient ? *Yes* but to be avoided for small problems example

## 4. Superlinear Time 
> mostly found in Divide and Conquer algos

Time Complexity: [ O(N log N) ]

examples:
1. Heap Sort
2. implementing Binary Search over an unsorted array ( We must sort and then search) 
3. Quick Sort 
4. Heap Sort

> Efficient ? *Yes* ! Algos with this time complexity are mostly used

## 5. Polynomial Time
> Generally for algos with a for loop inside a for loop.

Time Complexity: [ O (N ^ 2) ]

examples:
1. Bubble Sort
2. Insertion Sort
3. Selection Sort
4. Traversing a simple 2D array since there are two for loops ( one inside the other )

> Efficient ? *Partially Yes* These algorithm are mostly avoided unless an alternative algorithm of complexity O(N log N) is available.

## 6. Exponential Time
> An algorithm is said to be exponential time, if time taken by the algorithm is upper bounded by K ^ N

Time Complexity: [ O( N ^ K) ]

examples:
1. [Graph Isomorphism](https://en.wikipedia.org/wiki/Graph_isomorphism)
2. Travelling Salesman Problem using Dynamic Programming
3. O(10^N): trying to break a password by testing every possible combination (assuming numerical password of length N)

> Efficient ? *No* mostly avoid these until its very much needed

## 7. Factorial Time
> An algorithm with a time of upper bound N !

Time Complexity: [ O( N ! ) ]

examples:
1. Generate permutation of a list of length N ( which would take n!)
2. Naive bruteforce solution for Travelling Salesman problem

> Efficient? *No* ! Avoid them until you have no alternatives
