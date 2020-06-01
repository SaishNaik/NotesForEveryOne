# Summary

## LinkedList
The "runner" (or second pointer) technique is used in many linked list problems. The runner technique
means that you iterate through the linked list with two pointers simultaneously, with one ahead of the
other. The "fast" node might be ahead by a fixed amount, or it might be hopping multiple nodes for each
one node that the "slow" node iterates through.  
A number of linked list problems rely on recursion. If you're having trouble solving a linked list problem,
you should explore if a recursive approach will work.

## Stacks
Stacks are often useful is in certain recursive algorithms. Sometimes you need to push
temporary data onto a stack as you recurse, but then remove them as you backtrack (for example, because
the recursive check failed). A stack offers an intuitive way to do this.  
A stack can also be used to implement a recursive algorithm iteratively. (This is a good exercise! Take a
simple recursive algorithm and implement it iteratively.)

## Queues
It is especially easy to mess up the updating of the first and last nodes in a queue. 8e sure to double check
this.  
One place where queues are often used is in breadth-first search or in implementing a cache.

## Trees

A "balanced" tree really means something more like "not terribly imbalanced."lt's balanced enough to ensure 0( l o g n) times for i n s e r t and f i n d , but it's not necessarily as balanced as it could be.  
Two common types of balanced trees are red-black trees (pg 639) and AVL trees (pg 637).  
A complete binary tree is a binary tree in which every level of the tree is fully filled, except for perhaps the
last level. To the extent that the last level is filled, it is filled left to right.  
A full binary tree is a binary tree in which every node has either zero or two children. That is, no nodes have
only one child.  
A perfect binary tree is one that is both full and complete. All leaf nodes will be at the same level, and this
level has the maximum number of nodes.  
Traversal : in-order, post-order, and pre-order traversal. The most common of these is in-order traversal.  
Inorder: When performed on a binary search tree, it visits the nodes in ascending order (hence the name "in-order").  
Preorder: In a pre-order traversal, the root is always the first node visited.  
Postorder: the root is always the last node visited.  

## Heaps
A min-heap is a complete binary tree (that is, totally filled other than the rightmost elements on the last
level) where each node is smaller than its children. The root, therefore, is the minimum element in the tree. (max heap viceversa)  
Always implement min heap with a array.

Insert
When we insert into a min-heap, we always start by inserting the element at the bottom. We insert at the
rightmost spot so as to maintain the complete tree property. Then, we "fix" the tree by swapping the new element with its parent, until we find an appropriate spot forthe element. We essentially bubble up the minimum element.

Extract Minimum
First, we remove the minimum element and swap it with the last element in the heap (the bottommost,
rightmost element). Then, we bubble down this element, swapping it with one of its children until the min-
heap property is restored. The swap down should be done with smaller of its children to maintain min heap poperty.

Time Complexity O(logn)

## Tries (Prefix Trees)

A Trie is a nary tree. The * nodes (sometimes called "null nodes") are often used to indicate complete words. A node in a trie could have children  anywhere from 1 through ALPHABET_SIZE +1. +1 is for null nodes.

While a hash table can quickly look up whether a string is a valid word, it cannot tell us if a string is a prefix of any valid words. A trie can do this very quickly.A trie can check if a string is a valid prefix i n O ( K ) time, where K is the length of the string.


## Bits Manipulation

`a * 2` is shifting a to the left by 1.    
`a ^ (~a)` will give you 1 as all bits.  
`a & pow(2,n)` will result in last n bits to be 0. 

Recall that these operations occur bit-by-bit, with what's happening on
one bit never impacting the other bits. This means that if one of the above statements is true for a single bit,
then it's true for a sequence of bits.

Below s means series of 1

```
x ^ 0s = x  
x ^ 1s = ~x  
x ^ x = 0  
x & 0s = 0  
x & 1s = x  
x & x = x  
x | 0s = x  
x | 1s = 1s  
x | x = x  
```







