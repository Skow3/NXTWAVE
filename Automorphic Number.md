# Medium

# SOLUTION
```python
class solution:
    def checkAutomorphicNumber(self, num):
       return str(num**2)[-len(str(num)):] == str(num)
```
