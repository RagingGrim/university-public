# Binary Trees
A binary tree is a tree data structure in which each node has at most two children, which are referred to as the left child and the right child.

## Example
![No connection](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/Binary_tree.svg/192px-Binary_tree.svg.png)

A labeled binary tree of size 9 and height 3, with a root node whose value is 2. The above tree is unbalanced and not sorted.

## Types of binary Trees
### Full binary tree
A full binary tree (sometimes referred to as a proper or plane binary tree) is a tree in which every node in the tree has either 0 or 2 children.

![No connection](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Full_binary.pdf/page1-220px-Full_binary.pdf.jpg)
### Complete binary tree
In a complete binary tree every level, except possibly the last, is completely filled, and all nodes in the last level are as far left as possible

![No connection](https://upload.wikimedia.org/wikipedia/commons/thumb/8/85/Complete_binary.pdf/page1-220px-Complete_binary.pdf.jpg)

## Traversal
### breadth-first
breadth-first starts at the tree root and explores the neighbor nodes first, before moving to the next level neighbors.
This can be implemented as:
- top-down
- left-to-right
- right-to-left

![No connection](https://upload.wikimedia.org/wikipedia/commons/4/46/Animated_BFS.gif)

#### Performance
![No connection](https://wikimedia.org/api/rest_v1/media/math/render/svg/3723b61a52380fbdf4c6892af96ebbfe8fb76a22)

#### Code
```java
public void breadthFirst() {
  BSTNode<T> p = root;
  Queue<BSTNode<T>> queue = new Queue<BSTNode<T>>();

  if(p != null) {
    queue.enqueue(p);
    while (!queue.isEmpty()) {
      p = queue.dequeue();
      visit(p);
      if(p.left != null)
        queue.enqueue(p.left);
      if(p.right != null)
        queue.enqueue(p.right);
    }
  }
}
```
### depth-first
One starts at the root and explores as far as possible along each branch before backtracking.
