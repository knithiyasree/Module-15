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
```
<img width="1178" height="192" alt="image" src="https://github.com/user-attachments/assets/8004cde0-31cc-4d58-ac85-b292034665a9" />

```

## RESULT:
Thus a Python program to build and evaluate the given Expression tree has been executed successfully.

