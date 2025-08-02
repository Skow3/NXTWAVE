# Easy

# FINAL SOLUION:
```python
"""
class Node:
    def __init__(self, data, next=None, prev=None):
        self.data = data
        self.next = next
        self.prev = prev
"""

class solution:
    def deleteKthNode(self, Node, head, k):
        if not head or not head.next:
            return None
        if k==0:
            head = head.next
            head.prev = None
            return head
        ptr =head
        i=0
        while i!=k:
            ptr=ptr.next
            i+=1
        ptr.prev.next= ptr.next
        ptr.next.prev = ptr.prev
        return head
```
