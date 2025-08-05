# EASY

```python
class solution:
    def gcd(self, N, arr):
        def compute_gcd(a,b):
            while b!=0:
                a,b=b,a%b 
            return a
        result = arr[0]
        for i in range(1,N):
            result = compute_gcd(result,arr[i])
        return result
```
