# [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference)

**Solution**
<br>
```python
def diagonalDifference(arr):    
    return abs(sum((arr[i][i] - arr[i][-i-1] for i in range(len(arr)))))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
