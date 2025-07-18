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
    def deleteTail(self, Node, head):
        ptr = head
        if head == None:
            return None
        if head.next == None:
            return None
        while ptr.next.next:
            ptr = ptr.next
        ptr.next = None
        return head
`
```
