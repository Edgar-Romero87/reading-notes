# [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
## Binary Trees and Binary Search Tress

### Common Terminology
- **Node** - A node is the individual item/data that makes up the data structure
- **Root** - The root is the first/top `Node` in the tree
- **Left Child** - The node that is positioned to the left of a root or node
- **Right Child** - The node that is positioned to the right of a root or node
- **Edge** - The edge in a tree is the link between a parent and child node
- **Leaf** - A leaf is a node that does not contain any children
- **Height** - The height of a tree is determined by the number of edges from the root to the bottommost node.

## Traversals 
Depth and Breadth.
### Depth First
Depth first traversal is where we prioritize going through the depth (height) of the tree first. 

Methods for depth first traversal:
- Pre-order: `root >> left >> right`
```
ALGORITHM preOrder(root)
// INPUT <-- root node
// OUTPUT <-- pre-order output of tree node's values

    OUTPUT <-- root.value

    if root.left is not Null
        preOrder(root.left)

    if root.right is not NULL
        preOrder(root.right)
```      
- In-order: `left >> root >> right`
```
ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)
```
- Post-order: `left >> right >> root`
```
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

The most common way to traverse a tree is to use **recursion**, recursion occurs when a thing is defined in terms of itself or of its type.

### Breadth First
Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

Pseudocode utilizing a built-in queue to implement a breadth first traversal:
```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
```

## Binary Trees
Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our `left` and `right` children).


## Binary Search Trees
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the `root` are placed to the `left`, and all values that are larger than the `root` are placed to the `right`.


### Resources:

[Trees-Code Fellows](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)