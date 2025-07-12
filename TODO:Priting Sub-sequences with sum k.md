# Medium

Again a subsequence question .. solved using DFS

though will explain later on

# SOLUTION
```python
class solution:
    result = 0
    def findSubSequencesWithSumK(self, arr, n, k):
        self.dfs(0,arr,n,[],0,k)
        return self.result
        
    def dfs(self,index,arr,n,path,current_sum,target):
        if index==n :
            if current_sum == target:
                self.result+=1 
            return
        path.append(arr[index])
        self.dfs(index+1,arr,n,path,current_sum+arr[index],target)
        path.pop()
        self.dfs(index+1,arr,n,path,current_sum,target)
```
