# EASY 
Got an easy trick to call recursion in py

CODE:
```PYTHON
class solution:
    def recursionSum(self, N):
        if N==0:
            return 0
        return N+ self.recursionSum(N-1)
```

done
