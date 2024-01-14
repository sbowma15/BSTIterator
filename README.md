This Python program implements an iterator for a Binary Search Tree (BST) as part of Homework 06 in the CS3210 course. The iterator allows for in-order traversal of the BST, providing a way to iterate through the elements in ascending order.

BST Class
Constructor
The BST class represents a Binary Search Tree. It initializes the tree with a list of labels, ensuring the first label becomes the root node. Additional labels are added to the tree using recursion.

Methods
_add(node, label)
This private method adds a node with the given label to the BST using recursion.

_print(node, tabs = "")
A helper method that builds a string representation of the BST using recursion. It facilitates the visual representation of the tree.

__str__()
Overrides the default __str__ method to provide a string representation of the BST.

_in_order(node)
A helper method that builds a list with the elements of the BST in in-order order using recursion.

__iter__()
Implements the iterator protocol by returning self.

__next__()
Returns the label of the first element from the list built in __iter__, updating the list before returning. If the list is empty, an exception is thrown to indicate that there are no more elements to return.
