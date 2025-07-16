# EASY

# SOLUTION
```python
"""
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
"""

class solution:
    def insertionAtHead(self, Node, head, a):
        ptr = Node(a)
        ptr.next= head
        head = ptr
        return head
```
