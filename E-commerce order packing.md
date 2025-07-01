# Medium
Just applying concepts to real world

```python
class solution:
    orders = []
    def addOrder(self, itemName, quantity, price):
        self.orders.append({'itemName': itemName , 'quantity': quantity,'price': price })

    def updateOrder(self, itemName, newQuantity, newPrice):
        for orders in self.orders:
            if orders['itemName'] == itemName:
                orders['quantity'] = newQuantity
                orders['price'] = newPrice
                break
        pass  
    
    def calculateTotalRevenue(self):
        sumt = float(0)
        for orders in self.orders:
            sumt+=orders['quantity']*orders['price']
        return sumt
```

---
