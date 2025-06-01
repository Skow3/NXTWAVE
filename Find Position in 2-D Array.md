Lang : Python

```python
class solution:
    def searchElement(self, arr, n, m, k):
        r,c=-1,-1
        for i in range(0,n):
            for j in range(0,m):
                if arr[i][j]== k:
                    r,c = i,j
                    print(f"{r} {c}")
                    return 0
        print("-1 -1")
        pass
```

#### Note : Always use an early exit in your programs to save it from error in longer inputs
