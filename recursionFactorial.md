# EASY
Recursion is quite confusion topic for me no matter of how many times i revise and practise it.

Will try to add more and more practice to topics like :
1. Graphs
2. LinkedList
3. Different Techniques : Like memoization and all
4. Stacks
5. Heaps
6. Queues
7. Recursion

Soon i'll start doing topic-wise questions after covering from nextwave 

---

Coming back to this question :

# CODE
```python
class solution:
    def recursionFactorial(self, n):
        if n != 0:
            return n * self.recursionFactorial(n - 1)
        else:
            return 1
```
