# EASY

# FINAL SOLUTION
```python
"""
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
"""

class solution:
    def insertionBeforeX(self, Node, head, x, data):
        ptr = head
        new = Node(data)
        if head and head.data == x:
            new.next = head
            return new
        while ptr and ptr.next:
            if ptr.next.data == x:
                new.next = ptr.next
                ptr.next = new
                break
            ptr = ptr.next
        return head
```
