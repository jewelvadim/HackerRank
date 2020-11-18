# [Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem)

**Solution**
<br>
```python
def compareTriplets(a, b):
    
    result = [0, 0]
    
    for i in range(len(a)):
        if a[i] != b[i]:
            result[int(a[i] < b[i])] += 1
    
    return result
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
