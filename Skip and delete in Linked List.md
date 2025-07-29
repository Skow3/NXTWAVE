# EASY 

# FINAL SOLUTION:
```PYTHON
'''
class Node:
    def __init__(self, data=0, next=None):
        self.data = data
        self.next = next
'''

class solution:
    def deleteNAfterMNodes(self, Node, head, m, n):
        ptr =head
        while ptr.next:
            i=1
            while i!=m and ptr.next:
                ptr=ptr.next
                i+=1 
            i=0
            while i!=n:
                if ptr.next and ptr.next.next:
                    ptr.next = ptr.next.next
                else:
                    ptr.next = None
                    return head
                i+=1
            ptr = ptr.next
        return head
```
