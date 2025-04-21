# 📚 Stack Implementation using Linked List

This project is the **third assignment** for the GMT234 course. The goal is to implement a stack data structure using **linked lists**, and manage the development using **Git/GitHub workflows** such as branching and merging.

## 📁 Repository Structure


## 🌱 Branch Workflow

- A separate branch named `linked-list-stack` was created for the `ds.py` implementation.
- All related changes were committed under this branch.
- At least two commits were made before merging with the main branch.
- Merge was completed via GitHub.

## 📌 Task Summary

| Task                           | Status     |
|-------------------------------|------------|
| Transfer starter files        | ✅ Done     |
| Create branch                 | ✅ Done     |
| Implement Stack with Linked List | ✅ Done |
| Ensure `main_LL.py` works     | ✅ Done     |
| Make at least 2 commits       | ✅ Done     |
| Merge branch                  | ✅ Done     |
| Add README                    | ✅ Done     |

## 🧱 Class Overview

### 🔹 `Node` (Base Class)
Basic node with `data` and `next`.

### 🔹 `LinkedListNode` (Extends `Node`)
Inherits from `Node` and used in LinkedList-specific contexts.

### 🔹 `LinkedList`
A custom linked list implementation with methods:
- `add_node(node, index)` – Insert a node at given index
- `remove_node(index)` – Remove node at specified index

### 🔹 `Stack`
Implements stack behavior using the `LinkedList`:
- `push(node)` – Adds node to top of the stack
- `pop()` – Removes and returns the top node
- `peek()` – Returns (without removing) the top node

## 🔁 Stack Operations Example

```python
from ds import Stack, LinkedListNode

stack = Stack()
stack.push(LinkedListNode("A"))
stack.push(LinkedListNode("B"))

print(stack.peek().data)  # Output: B

stack.pop()
print(stack.peek().data)  # Output: A
