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
    def insertionAtTail(self, Node, head, a):
        new = Node(a)
        if not head:
            head = new
            return head
        if not head.next:
            head.next = new
            new.prev = head
            return head
        ptr = head
        while ptr.next:
            ptr=ptr.next
        ptr.next = new
        new.prev = ptr
        return head
```
