# [Cut the sticks](https://www.hackerrank.com/challenges/cut-the-sticks)

**Solution**
<br>
```python
def cutTheSticks(arr):
    res = []
    while arr:
        res.append(len(arr))
        m = min(arr)
        
        arr = [x for x in arr if x != m]

    return res
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
