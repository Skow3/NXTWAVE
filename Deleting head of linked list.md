# EASY

# FINAL SOLUTION:
```python
"""
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
"""

class solution:
    def deleteHead(self, Node, head):
        if head == None:
            pass
        elif head.next == None:
            head= None
            pass
        else:
            head = head.next
        return head
```
