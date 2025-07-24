# EASY

* Here i just applied the concept [peeche me aage wala , aage me dono jyda]

# FINAL SOLUTION
```python
class solution:
    def numOfways(self, n):
        if n==1 or n==0:
            return 1 
        a,b=1,1 
        for _ in range(2,n+1):
            a,b= b,a+b
        return b
```
