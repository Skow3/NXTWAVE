# EASY 

# FINAL SOLUTION
```PYTHON
"""
class Node:
    def __init__(self, data, next=None, prev=None):
        self.data = data
        self.next = next
        self.prev = prev
"""

class solution:
    def deletionAtTail(self, Node, head):
        if not head or not head.next:
            return 0
        ptr=head
        while ptr.next.next:
            ptr = ptr.next
        ptr.next.prev = None
        ptr.next = None
        return head
```
