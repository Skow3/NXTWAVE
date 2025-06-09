# EASY
```python
class solution:
    def reverseNumber(self, N):
        #Write your code here...
        k=0
        while N>0:
            k = k*10 + N%10
            N//=10
        return k
        pass
```
