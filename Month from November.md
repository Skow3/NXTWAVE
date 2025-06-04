# Easy

#### THINGS REVISED 
Using Dictionary and simulating switch using get 

```python
class solution:
    def getMonthName(self, monthNumber):
        switch = {
            1: "January",
            2: "February",
            3: "March",
            4: "April",
            5: "May",
            6: "June",
            7: "July",
            8: "August",
            9: "September",
            10: "October",
            11: "November",
            12: "December",
        }
        print(switch.get(monthNumber, "Invalid input!"))
```
