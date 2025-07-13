# MEDIUM

Tho it was marked as medium but in python it was easy by just returning x**n and it handles decimal by itself.

---

# SOLUTION
```python
class solution:
    def xPowN(self, x, n):
        return x**n
```

But in C++

# CPP SOLUTION
```cpp
#include <bits/stdc++.h>
using namespace std;

class solution {
    public:
    double xPowN(double x, long long n) {
        if (n==0) return 1;
        bool isNegative = (n<0);
        n=abs(n);
        double result =1;
        while (n>0){
            if(n%2==1){
                result*=x;
            }
            x*=x;
            n/=2;
        }
    
        return isNegative ? 1.0/result : result;
    }
};
```
