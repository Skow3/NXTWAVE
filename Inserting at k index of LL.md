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
    def insertionAtKthPosition(self, Node, head, k, data):
        if k ==0:
            ptr= Node(data)
            ptr.next = head
            head= ptr
            return head
        if head == None:
            return None
        i=0
        ptr = head
        new = Node(data)
        while i!=k-1:
            ptr = ptr.next
            i+=1
        new.next = ptr.next
        ptr.next = new
        return head
```
