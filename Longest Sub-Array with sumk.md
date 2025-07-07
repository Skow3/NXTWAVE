# MEDIUM

# APPROACH 1 [ USING DIFFERENCE ]
```python
n = 4
k = -5
arr = [-1,-2,-3,-4]
i=0
lent =0
mas =0
while i<n:
    d= k
    j=i
    lent =0
    while j<n and (d>= 0 or (k<0 and d<=0)):
        print(f"{i} {j} {d}")
        if d == 0 :
            mas = max(mas,lent)
            print(f" THIS IS MAS :{i},{mas}")
            break
        else:
            d= d-arr[j]
            lent+=1
        j+=1
    i+=1
print(mas)
```
PASSED 88% 

# FINAL SOLUTION
```python
# USING SUM
class Solution:
    def longestSubarrayWithSumK(self, arr, n, k):
        mas = 0
        for i in range(n):
            summ = 0
            for j in range(i, n):
                summ += arr[j]
                if summ == k:
                    mas = max(mas, j - i + 1)
        return mas
```

---

