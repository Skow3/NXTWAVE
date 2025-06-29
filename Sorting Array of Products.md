# Medium 
though it was easy

# SOLUTION

```python
class solution:
    def sortProducts(self, products):
        return sorted(products,key=lambda x: x[1])
    
    def displayProducts(self, products):
        hj = self.sortProducts(products)
        for i in hj:
            print(f"{i[0]}:{i[1]}")
        pass
```
