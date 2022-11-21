# [Breaking the Records](https://www.hackerrank.com/challenges/breaking-best-and-worst-records)

**Solution**
<br>
```python
def breakingRecords(scores):
    min_ = max_ = scores[0]
    
    result = [0, 0]
    
    for i in scores:
        if i > max_:
            max_ = i
            result[0] += 1
        elif i < min_:
            min_ = i
            result[1] += 1
            
    return result
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
