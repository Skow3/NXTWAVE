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
    def searchInLL(self, Node, head, k):
        ptr = head
        i=1
        while ptr:
            if ptr.data == k:
                return 1
            ptr = ptr.next
            i+=1
        return 0
```
