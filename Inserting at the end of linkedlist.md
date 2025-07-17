# EASY 

# SOLUTION

```PYTHON
"""
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
"""

class solution:
    def insertionAtTail(self, Node, head, a):
        ptr = head
        if head == None:
            head = Node(a)
            return head
        while ptr.next:
            ptr = ptr.next
        ptr.next = Node(a)
        ptr= ptr.next
        return head
```
