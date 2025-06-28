# EASY
The question was easy but i was stuck in some error 
later on on deeply recoginzing i had the opposite condition in the while loop

# SOLUTION
```python
class Solution():
  def setzeroes(self,arr,n):
    count=0
    for i in arr:
      if i!=0:
        arr[count]=i
        count+=1
    while count<n:
      arr[count] = 0
      count+=1
    return arr
```
# DONE
