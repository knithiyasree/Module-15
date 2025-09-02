# Ex. No: 15A - Build  a binary search tree using a built in function

## AIM:
To Debug a Python program to build a binary search tree using a built in function

1. Use appropriate module to build a binary tree

2. def _build_bst_from_sorted_values(sorted_values):  - to build a binary search tree for the below given tree.

3. def insert_BST(val): - to insert a node value and rebuilt a BST , get the value to be inserted from the user and pass it to the function.

4. def display(T): - to display the values of the tree nodes
---

## ALGORITHM:

Here you go in clean **copy format** 👇

---

**Algorithm**

1. Start the program.
2. Import the `Node` class from the `binarytree` module.
3. Define functions to build a BST from a sorted list, insert a new value, and display the BST.
4. Initialize the list `x = [5,3,6,2,4,1]`.
5. Build and display the BST before insertion.
6. Read input value `s` from the user.
7. Insert `s` into the BST and display the updated tree.
8. End the program.

---

## PYTHON PROGRAM

```
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    
    if len(sorted_values) == 0:
        return None
    mid_index = len(sorted_values) // 2
    root = Node(sorted_values[mid_index])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right = _build_bst_from_sorted_values(sorted_values[mid_index + 1 :])  
    return (root)

def insert_BST(val):
  global x
  if val in x:
    return False
  else:
    x.append(val)
  tree=_build_bst_from_sorted_values(sorted(x))
  return tree

def display(T):
    for i in T.values:
        print(i,"-->",end="")

x=[5,3,6,2,4,1]
print("BST before insertion:")
t=_build_bst_from_sorted_values(sorted(x))
display(t)
s=int(input())
print("\nBST after insertion: ")
t1=insert_BST(s)
display(t1)


```

## OUTPUT
<img width="853" height="225" alt="image" src="https://github.com/user-attachments/assets/7e5257f7-7b85-4abc-9fc0-451d957c9c6c" />


## RESULT
Thus a Python program to build a binary search tree using a built in function has been executed successfully.
