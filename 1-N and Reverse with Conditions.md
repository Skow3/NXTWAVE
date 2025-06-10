# EASY

---

This is the code , wrote the code in cpp to refresh some concepts:

```cpp
#include <bits/stdc++.h>
using namespace std;

class solution{
    public:
    void printEvenOdd(int n) {
        if(n>2){
        for(int i=2;i<=n; i=i+2){
            std::cout << i << " ";
        }
        }
        int i=0;
        if(n%2==0){
            i = n-1;
        }
        else{
            i = n;
        }
        for(i;i>0;i=i-2){
            cout<< i << " ";
        }
        
    }
};
```
