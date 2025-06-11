# EASY

Learnt a nice concept :
Since we know that HCF*LCM =  Product of two numbers 

Therefore we can find the LCM after finding the HCF of the given numbers

```python
class solution:
    def lcm(self, A, B):
        #Write your code here...
        a,b = A,B
        while b!=0:
            a,b= b,a%b
        return int(A*B)//a
```

