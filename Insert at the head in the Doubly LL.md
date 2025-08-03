# EASY 

# FINAL SOLUTION
```python
"""
class Node:
    def __init__(self, data, next=None, prev=None):
        self.data = data
        self.next = next
        self.prev = prev
"""

class solution:
    def insertionAtHead(self, Node, head, a):
        new = Node(a)
        if not head:
            head = new
            return head
        ptr = head
        new.next = ptr
        ptr.prev = new
        new.prev = None
        head = new
        return head
```
