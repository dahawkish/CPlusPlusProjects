Here is a file about explaining completed tree.

Thought: I think the professor gave us a lot of examples about completed trees but somehow, understanding the definition is more important.

1. You need to know that a completed tree might exist in more than a binary search tree or binary tree. 

Thought: a lot of data structures courses would introduce binary tree or binary search tree from the beginning, and if you/
were a math major with some topology background, would have some doubts. It is ok if you over-think, but I try to explain/
here with my understanding. (let me know if I am wrong....)

Tip: ask your professor if he/she is only talking about completed Binary Search Tree/Binary Tree.

2. About a completed binary search tree/binary tree:
Tip: think about if a BST/BT is a completed tree from as a programmer

1) find the root, if the root is null, then it is a completed BST/BT?

Tip: A BST/BT can have only one node, which is the root.

a. if yes, return arr[] is empty.

b. if not, enqueue.arr[0].

2) search the 1st level of the tree if you assume 0 level has only the root:

a. there are at most 2 children under the root, and enqueue arr[1] and arr[2];
b. if enqueue arr[1]=NULL, this is still a completed tree without children.
c. if enqueu arr[1] is not NUll, it is still a complete tree without the right child;

3) writing a searchChild function using link list and enqueue.

Tips: there are many ways to traverse a tree, and I am using BFS here.

4) search the 2rd level of the tree

Tips: from the 2), there is a pattern from 2) based on the same level. 
a. search if there is a child
b. if leftChild is NULL, check if there is right child. 
c. if there is left child, we need to know if ther eis more than one right child. 
d. if ther eis more than one right child, we need to fill the all the left children on the same level. 
