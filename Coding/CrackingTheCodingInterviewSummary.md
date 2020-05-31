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
