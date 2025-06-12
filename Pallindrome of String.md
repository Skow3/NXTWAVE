# EASY 

Checking for pallindrome ...

Start from checking the last and the first letter of the string and returning true /false

---

```python
class solution:
    def checkPalindrome(self, s):
        l=0
        r= len(s)-1
        while l < r:
            if s[l] != s[r]:
                return False
            r-=1
            l+=1
        return True
```

---
