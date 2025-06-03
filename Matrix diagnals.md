# EASY 

```pyhon
class solution:
    def sumOfDiagonals(self, matrix, n):
        suml=0
        sumr=0
        for i in range(n):
            sumr+= matrix[i][i]
            suml+= matrix[i][n-1-i]
        print(sumr,suml)
        pass
```

