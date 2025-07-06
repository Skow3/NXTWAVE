# EASY
Just like we did Moving zeroes to end.
This time going reverse direction.

# SOLUTION
```python
class solution:
    def moveZerosToFront(self, arr, n):
        i= len(arr) -1
        g= i
        while i !=-1:
            if arr[i] != 0:
                arr[g]= arr[i]
                g-=1 
            i-=1 
        while g!=-1:
            arr[g]=0
            g-=1
        pass
```
