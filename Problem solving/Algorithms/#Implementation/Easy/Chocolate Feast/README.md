# [Chocolate Feast](https://www.hackerrank.com/challenges/chocolate-feast/problem)

**Solution**
<br>
```python
def chocolateFeast(n, c, m):
    choclates = n // c
    wrappers = choclates
    
    while wrappers >= m:
        choclates += wrappers // m
        wrappers = wrappers // m + wrappers % m
        
    return choclates
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
