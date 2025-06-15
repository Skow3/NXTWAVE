# EASY
Though it was easy it took sometime for me to get a grip over the solution [Maybe bcs i was busy in some other work too]

---

#### CODE 1
```python
class solution:
    def calculateDigitSum(self,N1, N2):
        sumt =0
        for i in range(N1,N2+1):
            print(i)
            sumt += int(str(i)[0])+ int(str(i)[1])
        return sumt
```

##### Do you think that everything is right there?
---> No, i forgot to take the cases where there can be 1 digit numbers only example(4,9)

##### CODE 2
```PYTHON
class solution:
    def calculateDigitSum(self,N1, N2):
        sumt =0
        for i in range(N1,N2+1):
            if len(str(i)) ==1:
                sumt+= int(str(i)[0])
            else:
                sumt += int(str(i)[0])+ int(str(i)[1])
        return sumt
```

##### Do you think that this is correct now?
---> No, i forgot to take the other digit cases for example (456...,234...)

So finally did some changes =>

# FINAL SOLUTION
```python
class solution:
    def calculateDigitSum(self,N1, N2):
        sumt =0
        for i in range(N1,N2+1):
            digits = str(i)
            sumt += sum(int(d) for d in digits)
        return sumt
```
