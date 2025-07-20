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
    def deleteKthNode(self, Node, head, k):
        if head == None or head.next==None:
            return None
        ptr = head
        i=0
        while i!= k-1:
            ptr = ptr.next
            i+=1
        ptr.next = ptr.next.next
        return head
```
