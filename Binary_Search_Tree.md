

# Binary Search


## Question : 

Write the Binary-Search-Tree steps of the list [7, 5, 1, 8, 3, 6, 0, 9, 4, 2].


## Answer

Step 1: Create the root node with the first element of the list, in this case, 7. The binary search tree now looks like this:

```
7
```

Step 2: Compare the second element of the list, 5, to the root node. Since 5 is less than 7, it is added as a left child to the root node. The binary search tree now looks like this:

```
    7

   /

  5
```

Step 3: Compare the third element of the list, 1, to the root node and its children. Since 1 is less than 5, it is added as a left child to the 5 node. The binary search tree now looks like this:

```
    7

   /

  5  

 /

1
```

Step 4: Compare the fourth element of the list, 8, to the root node and its children. Since 8 is greater than 7, it is added as a right child to the root node. The binary search tree now looks like this:

```
    7

   / \

  5   8

 /

1
```

Step 5: Compare the fifth element of the list, 3, to the root node and its children. Since 3 is less than 5, it is added as a left child to the 1 node. The binary search tree now looks like this:

```
    7

   / \

  5   8

 /  

1

 \

  3
```

Step 6: Compare the sixth element of the list, 6, to the root node and its children. Since 6 is greater than 5 and less than 7, it is added as a right child to the 5 node. The binary search tree now looks like this:

```
    7

   / \

  5   8

 /  \

1   6

 \

  3
```

Step 7: Compare the seventh element of the list, 0, to the root node and its children. Since 0 is less than 1, it is added as a left child to the 1 node. The binary search tree now looks like this:

```
        7

       / \

      5   8

     /  \

    1   6

    /

   0

     \

      3
```

Step 8: Compare the eighth element of the list, 9, to the root node and its children. Since 9 is greater than 8, it is added as a right child to the 8 node. The binary search tree now looks like this:

```
        7

       / \

      5   8

     /       \

    1        9

    /

   0

   \

    3
```

Step 9: Compare the ninth element of the list, 4, to the root node and its children. Since 4 is greater than 3 and less than 5, it is added as a right child to the 3 node. The binary search tree now looks like this:

```

        7

       / \

      5   8

     /       \

    1        9

    /

   0

   \

    3

       \

        4
```

Step 10: Compare the tenth element of the list, 2, to the root node and its children. Since 2 is less than 3, it is added as a left child to the 3 node. The binary search tree now looks like this:

```

        7

       / \

      5   8

     /       \

    1        9

    /

   0

      \

       3

      /   \

     2    4
```

At this point, the binary search tree is fully constructed and all elements of the list have been added to the tree according to the binary search tree rules, which state that for each node, the left child contains elements that are smaller than the node and the right child contains elements that are greater than the node.

It's also worth noting that the binary search tree is not sorted and the elements might not be in the same order as the input list, but it's still a valid representation of the input data and it can be used for searching, insertion and deletion operations.

The time complexity of building a binary search tree is O(n*log(n)) on average because each insertion or deletion operation takes log(n) time on average to find the correct position to insert or delete the element.

The space complexity is O(n) as it requires space to store each element in the tree.
