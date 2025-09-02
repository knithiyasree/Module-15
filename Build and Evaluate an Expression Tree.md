# Ex. No: 15E - Build and Evaluate an Expression Tree

## AIM:
To write a Python program to build and evaluate the given Expression tree.

---

## ALGORITHM:

1. **Start the program.**
2. Create nodes for operators and operands.
3. Build the expression tree by connecting nodes in the correct hierarchical structure.
4. Define a recursive function `evaluate(root)`:
   - If the node is a number (leaf), return it.
   - Else, recursively evaluate left and right subtrees.
   - Apply the operator at the current node to the results.
5. Return the final result from the root node.
6. **End the program.**

---

## PROGRAM:

```
from binarytree import build
x=['/','*','+',"+",4,'-',2,3,1,None,None,9,5,None,None]
exp=build(x)
print(exp.inorder)
print(exp.postorder)
```

## OUTPUT:
<img width="1179" height="193" alt="Screenshot 2025-09-02 202416" src="https://github.com/user-attachments/assets/113d9e2f-16c8-4d1a-b2e1-19cd2a088561" />


## RESULT:
Thus a Python program to build and evaluate the given Expression tree has been executed successfully.

