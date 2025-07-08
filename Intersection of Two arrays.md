# EASY 

This was a easy question with very less constraints 
But i got to know one thing today which i'll tell in the end

# SOLUTION 1
```PYTHON
class solution:
    def intersectionSortedArrays(self, a, b):
        dt= dict()
        for i in a:
            if i not in dt:
                dt[i] = 1 
            else:
                dt[i]+=1 
        ans = []
        for i in b:
            if i in dt and dt[i] > 0:   # SEE HERE WE ARE CHECKING FOR I IN DT
                ans.append(i)
        return ans
```

Not checking for i in dt will result in a keyerror

---


Though when we will use Counter i.e

```python
from collections import Counter

def intersect(nums1, nums2):
    count1 = Counter(nums1)
    result = []
    
    for num in nums2:
        if count1[num] > 0:
            result.append(num)
            count1[num] -= 1
            
    return result
```

Here we are not checking bcs i got to know that the Counter is a special type of dict
* It returns 0 when an index is not found // instead of an keyerror

