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
    def arrayToLL(self, Node, n, arr):
        if n==0:
            return 0
        head = Node(arr[0])
        ptr = head
        i=1
        while i < n:
            new = Node(arr[i])
            ptr.next = new
            ptr=new
            i+=1
        return head
```
