## EASY 

```python
class solution:
    def printPattern(self, n):
        i=1
        while i!=n+1:
            for _ in range(i):
                if _ < i-1:
                    print("*",end="")
                else:
                    print("*")
            i+=1
        pass
```

