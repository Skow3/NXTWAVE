# EASY

# Solution [just by using in]
```python
class Solution:
    def kthMissingNumber(self, arr, k):
        missing_count = 0
        prev = 0  # Assuming the sequence starts from 1

        for num in arr:
            gap = num - prev - 1  # Count numbers missing between prev and current num
            if missing_count + gap >= k:
                return prev + (k - missing_count)
            missing_count += gap
            prev = num

        # If kth missing is beyond the last element
        return arr[-1] + (k - missing_count)
```

# MORE OPTIMIZED VERSION

By doing the missing count

```PYTHON
class Solution:
    def kthMissingNumber(self, arr, k):
        missing_count = 0
        prev = 0  # Assuming the sequence starts from 1

        for num in arr:
            gap = num - prev - 1  # Count numbers missing between prev and current num
            if missing_count + gap >= k:
                return prev + (k - missing_count)
            missing_count += gap
            prev = num

        # If kth missing is beyond the last element
        return arr[-1] + (k - missing_count)
```
