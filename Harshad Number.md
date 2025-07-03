# EASY 

* A number is called Harshad Number if it is divisible by the sum of its digits.

# SOLUTION
```python
class solution:
    def checkHarshadNumber(self, num):
        sumt=0
        for i in str(num):
            sumt+= int(i)
        return num%sumt == 0
```
