# MEDIUM

The question was to check each digit of the number and return true if all of them are even

Did the question by using int and str conversion techniques.

```python
class solution:
    def checkEvenDigits(self, num):
        for i in str(num):
            if int(i)%2!=0:
                return False
        return True
```

Time complexity: O(d)
Space complexity : O(d)
