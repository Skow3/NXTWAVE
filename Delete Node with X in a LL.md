# EASY

---

# FINAL SOLUTION
```python
"""
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
"""

class solution:
    def deleteNodeWithValueX(self, Node, head, x):
        ptr=head
        if not head:
            return None
        if head.data == x:
            if head.next:
                head=head.next
                pass
            return 0 
        while ptr.next.data!=x :
            ptr=ptr.next
        ptr.next = ptr.next.next
        return head
```
