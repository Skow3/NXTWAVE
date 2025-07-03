# MEDIUM

### ARMSTRONG NUMBER IS A NUMBER :
Such that the sum of the individual digits of the number raised to the power of number of digits in num then it is true.

# SOLUTION
```python
class solution:
    def checkArmstrongNumber(self, num):
        sumt=0
        for i in str(num):
            sumt+= pow(int(i),len(str(num)))
        return sumt==num
```
