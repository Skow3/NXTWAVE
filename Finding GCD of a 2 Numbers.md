# EASY

---

##### This is purely that euclid's division formula based thing 
though i will always remember this bcs this can be later on used to find the lcm too

# SOLUTION:
```python
class solution:
  def findgcd(self,A,B):
    while B!=0:
      B,A = A%B,B
    return A
```

That's it and we're done
