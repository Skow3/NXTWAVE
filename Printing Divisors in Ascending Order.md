# EASY 
So this question was easy to understand and to implement but the thing here which was important was the optimization:

So these were the different approaches / solution i thought of :

# SOLUTION 1 :
```PYTHON
class Solution:
    def printDivisors(self, n):
        for i in range(1,n+1):
            if n%i==0:
                print(i,end=" ")
```

* Casual printing and coding right?

Now 
# SOLUTION 2 :
```PYTHON
class solution:
    def printDivisors(self, n):
        return [i for i in range(1,n+1) if n%i==0]
```

* SOMEWHAT INTERESTING ONE-LINER

Now let's go with the optimization 
```python
class solution:
    def printDivisorsopt(self, n):
        divisors = set()   # Making a set for storing the numbers
        for i in range(1, int(n**0.5) + 1):
            print(f'I  = {i}') ## used for testing
            if n % i == 0:
                divisors.add(i)
                divisors.add(n // i)    ## // operator gives us the divisor [Example 81//3 = 27]
            print(divisors)
        for d in sorted(divisors):
            print(d, end=" ")
```

GREAT LEARNING QUESTION
