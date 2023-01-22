
# Binary Search


## Question : 

Write the Binary-Search-Tree steps of the list [7, 5, 1, 8, 3, 6, 0, 9, 4, 2].


## Answer

here's how the binary search tree would look like if the first element of the list, 7, was chosen as the root, with more detailed explanations for each step:

Step 1: Create the root node of the tree with the first element of the list, which is 7. The tree now looks like:

    7

Step 2: Compare the next element in the list, 5, to the root node. Since 5 is less than 7, it is added as the left child of the root node. The tree now looks like:

    7

   /

  5

Since 5 is less than 7, it is added as a left child to the root node 7. This is because in a binary search tree, elements less than the root node are stored in the left subtree, and elements greater than the root node are stored in the right subtree.

Step 3: Compare the next element in the list, 1, to the root node and its children. Since 1 is less than 5, it is added as the left child of the 5 node. The tree now looks like:

    7

   /

  5

 /

1

In this step, we continue to compare 1 to the nodes in the tree, and we find that 1 is less than 5. Therefore, it is added as a left child to the 5 node, which is already a left child of the root node 7.

Step 4: Compare the next element in the list, 8, to the root node and its children. Since 8 is greater than 7, it is added as the right child of the root node. The tree now looks like:

    7

   / \

  5   8

 /

1

Here, we find that 8 is greater than 7, so it is added as a right child to the root node 7.

Step 5: Compare the next element in the list, 3, to the root node and its children. Since 3 is less than 5, it is added as the left child of the 5 node. The tree now looks like:

    7

   / \

  5   8

 / \

1   3

We continue to compare 3 to the nodes in the tree, and we find that 3 is less than 5. Therefore, it is added as a left child to the 5 node, which is already a left child of the root node 7.

Step 6: Compare the next element in the list, 6, to the root node and its children. Since 6 is greater than 5 and less than 8, it is added as the right child of the 5 node. The tree now looks like:

    7

   / \

  5   8

 / \  

1   3  6

Explanation: Now we compare 6 to the nodes in the tree, we find that it is greater than 5 and less than 8, so it is added as a right child to the 5 node.

Step 7: Compare the next element in the list, 0, to the root node and its children. Since 0 is less than 1, it is added as the left child of the 1 node. The tree now looks like:

        7

       / \

      5   8

     / \  

    1   3  6

   /

  0

We find that 0 is less than 1, so it is added as a left child to the 1 node, which is already a left child of the 5 node.

Step 8: Compare the next element in the list, 9, to the root node and its children. Since 9 is greater than 8, it is added as the right child of the 8 node. The tree now looks like:

        7

       / \

      5   8

     / \  

    1   3  6

   /      \

  0        9

We find that 9 is greater than 8, so it is added as a right child to the 8 node, which is already a right child of the root node 7.

Step 9: Compare the next element in the list, 4, to the root node and its children. Since 4 is greater than 3 and less than 5, it is added as the right child of the 3 node. The tree now looks like:

        7

       / \

      5   8

     / \  

    1   3  6

   /    /

  0    4

We find that 4 is greater than 3 and less than 5, so it is added as a right child to the 3 node, which is already a left child of the 5 node.

Step 10: Compare the next element in the list, 2, to the root node and its children. Since 2 is less than 1, it is added as the left child of the 1 node. The tree now looks like:

        7

       / \

      5   8

     / \  

    1   3  6

   /    /

  0    4

 /

2

We find that 2 is less than 1, so it is added as a left child to the 1 node, which is already a left child of the 5 node.

As you can see the tree is built in a way that the elements are sorted in a way that the left subtree of any node contains elements lesser than the node itself, and the right subtree contains elements greater than the node itself. This is the property that makes a binary search tree useful for searching and sorting elements. The time complexity of searching for an element in a binary search tree is O(log n), where n is the number of elements in the tree.
