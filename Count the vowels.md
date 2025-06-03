# EASY 


class solution:
    def countVowels(self, strs):
        c=0
        v = {'a','e','i','o','u'}
        for i in strs.lower():
            if i in v:
                c+=1
        return c

---

## POINTS TO NOTE:
While handling with strings always keep cases similar
