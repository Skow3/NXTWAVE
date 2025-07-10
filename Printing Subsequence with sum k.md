# EASY 
Again a subseqeunce question...

# SOLUTION
```PYTHON
class solution:
    def findSubSequencesWithSumK(self, arr, n, k):
        result = []
        self.dfs(0,arr, n,[],0,k,result)
        return result
        
    def dfs(self,index,arr,n,path,current_sum,target,result):
        if index == n:
            if current_sum == target:
                result.append(path[:])
            return
        path.append(arr[index])
        self.dfs(index+1,arr,n,path,current_sum+arr[index],target,result)
        path.pop()
        self.dfs(index+1,arr,n,path,current_sum,target,result)
```

Here I'm using DFS, to select and deselect the number.

![dfs](https://github.com/user-attachments/assets/6318ffe3-c5fd-42b6-87eb-7017f4787cad)

Will explain it more on Monday
