# [Migratory Birds](https://www.hackerrank.com/challenges/migratory-birds)

**Solution**
<br>
```python
def migratoryBirds(arr):
    result = [0] * (len(arr) + 1)
    
    for i in arr:
        result[i] += 1
        
    return result.index(max(result))
```

**Solution in one iteration**
<br>
```python
def migratoryBirds(arr):
    result = [0] * (len(arr) + 1)
    max_ = 0
    index = max(arr) + 1
    
    for i in arr:
        result[i] += 1
        
        if result[i] > max_:
            max_ = result[i]
            index = i
        elif result[i] == max_ and i < index:
            index = i
        
    return index
```


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
