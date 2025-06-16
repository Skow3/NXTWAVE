# EASY BUT TOOK TIME BECAUSE OF QUESTION MIS-INTERPRETATION

In this question we have to find out the LCM MODULO By 10<sup>9</sup>+7 therefore if the LCM is very large still the result would be small

```python
class solution:
    def lcmArray(self, arr):
        MOD = 10**9 +7 ## this was the thing i was missing 
        def gcd(x,y):
            while y:
                x,y = y, x%y
            return x
        
        def lcm(x,y):
            return (x)//gcd(x,y) * y % MOD
        result = arr[0]
        for i in arr[1:]:
            result = lcm(result,i)
        return result

```
