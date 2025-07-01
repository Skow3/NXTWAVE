# Medium
* This problem told me about `defaultdict`

---

# SOLUTION:
```python
from collections import defaultdict

class solution:
    def countWords(self, wordCount, paragraph):
        counts =defaultdict(int)
        for word in paragraph.split():
            counts[word]+=1
        self.displayWordCount(counts)
        pass
    
    def displayWordCount(self, wordCount):
        for word,count in sorted(wordCount.items(),key=lambda x:x[0]):
            print(f"{word}-{count}")
        pass
```
