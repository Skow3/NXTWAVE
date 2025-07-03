# EASY

This was a easy question i, though i forgot the optimized version to find the factors of a number.

## PERFECT NUMBER:
* It is a number in which the sum of it's factors [ not including itself ofc] == number itself.

----> How to find the factors of a number optimized version
```python
  nums = 30
  divisors  = set()
  for i in range(1,int(nums**0.5)+1):
    if n%i==0:
      divisors.add(i)
        if i!=1:
          divisors.add(n//i)
  return divisors
```

# SOLUTION:
```python
class solution:
    def checkPerfectNumber(self, num):
        div  = set()
        for i in range(1,int(num**0.5)+1):
            if num%i==0:
                div.add(i)
                if i!=1:
                    div.add(num//i)
        return sum(div) == num
```

---


      
