# EASY

Got to know some knew tricks concepts while experimenting

---

In python we can use [::-1] for reversing an array [Doesn't modify the original one]

So now ... The 2 codes which i wrote were

```python
class solution:
    def reverse(self, arr, N):
        arr.reverse()   # Using BIF
        return arr
```

```python
class solution:
    def reverse(self, arr, N):
        ans = arr[::-1]
        return ans
```
