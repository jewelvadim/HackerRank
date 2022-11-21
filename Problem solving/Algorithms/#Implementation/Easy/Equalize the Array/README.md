# [Equalize the Array](https://www.hackerrank.com/challenges/equality-in-a-array)

**Solution**
<br>
```python
def equalizeArray(arr):
    return len(arr) - max(arr.count(x) for x in set(arr))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
