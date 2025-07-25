# EASY 

# BUSY IN HACKATHON

```python
class solution:
    def minEnergy(self, n, height):
        if n==0:
            return 0
        dp = [0]*n
        dp[0] = 0
        dp[1] = abs(height[1]- height[0])
        for i in range(2,n):
            first = dp[i-1]+ abs(height[i]- height[i-1])
            second = dp[i-2]+ abs(height[i]- height[i-2])
            dp[i] = min(first,second)
        return dp[n-1]
```
