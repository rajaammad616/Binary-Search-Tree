Binary Search Tree (BST) in C++
This C++ program demonstrates the implementation of a Binary Search Tree (BST). It allows users to perform basic tree operations such as inserting, searching, deleting nodes, printing the tree in level-order (BFS), and finding the height of the tree. The implementation includes both recursive and iterative approaches for certain functionalities.

**Features**
Insert a node into the BST (recursively)
Search for a node (both recursive and iterative search used)
Delete a node (handling all 3 cases: leaf, one child, two children)
Print the tree using Level-Order Traversal (Breadth-First Search)
Compute the height of the tree
Cross-platform screen clearing (Windows/Linux support)

**Class Overview**

  **TreeNode Class**
  Represents a node in the BST.
  **Attributes:**
      int value
    TreeNode* left
    TreeNode* right
  **Constructors:**
    Default constructor
    Parameterized constructor with value

  **BST Class**
  Encapsulates the logic of Binary Search Tree operations.
  **Attributes:**
    TreeNode* root
  **Functions:**
    isTreeEmpty(): Check if the BST is empty
    insertRecursive(TreeNode*, TreeNode*): Insert a node recursively
    iterativeSearch(int): Iteratively search for a node
    height(TreeNode*): Calculate tree height
    printLevelOrderBFS(TreeNode*): Print nodes level by level
    printGivenLevel(TreeNode*, int): Helper for BFS
    minValueNode(TreeNode*): Find node with minimum value (used in deletion)
    maxValueNode(TreeNode*): Find node with maximum value
    deleteNode(TreeNode*, int): Delete a node from the BST

**Menu Options**

After running the program, a menu will be shown:

Option	Operation

1	Insert Node

2	Search Node

3	Delete Node

4	Print/Traversal BST

5	Height of Tree

6	Clear Screen

0	Exit Program

 **Notes**
  Memory Management: All nodes are dynamically allocated using new. Manual memory cleanup isn't included at the end of main() but can be added if needed.
  Search: Uses both iterative and recursive versions for practice and flexibility.
  Cross-Platform Compatibility: Screen clearing uses system("cls") for Windows and system("clear") for Unix/Linux.

