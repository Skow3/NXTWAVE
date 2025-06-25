#  EASY
Got a nice trick to find the unique single element in an array .

---

# FIRST APPROACH
Using mapping
```python
class solution:
    def findSinglEelement(self, arr, n):
        s = {}
        for i in arr:
            if i not in s:
                s[i] = 0
            else:
                s[i] +=1
        for key,values in s.items():
            if values ==0:
                return key
```

# SECOND APPROACH :
Using XOR
since we now that XOR gives this table
![image](https://github.com/user-attachments/assets/f5afcdae-002b-4dd4-a606-abb8134ef6d0)
i.e For XOR if the number is XORED with itself it returns 0

Otherwise it remains same 
So if the number will come twice then this will be cancelled out.

Though this method cannot be used if there are more than 2 repetitions [more precisely odd repetitions]
