# EASY

# SOLUTION
```python
class solution:
    def fib(self, n):
        if n == 0:
            return 0
        if n== 1:
            return 1
        his=0
        pis=1
        i=1
        while i != n:
            tis = his+pis 
            his = pis 
            pis = tis
            i+=1
        return pis
```
