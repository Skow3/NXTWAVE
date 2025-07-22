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
    def traversal(self, Node, head):
        while head:
            print(head.data,end=" ")
            head = head.next
        pass
```
