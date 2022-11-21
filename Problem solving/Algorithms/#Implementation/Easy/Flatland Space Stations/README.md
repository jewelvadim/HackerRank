# [Flatland Space Stations](https://www.hackerrank.com/challenges/flatland-space-stations)

**Solution**
<br>
```python
def flatlandSpaceStations(n, c):
    if len(c) == n:
        res = 0
    else:
        c.sort()
        res = max([c[0], n - 1 - c[-1]])
        
        if len(c) > 1:
            for i in range(len(c) - 1):
                
                d = (c[i+1] - c[i]) // 2
                
                if d > res:
                    res = d
                    
    return res
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
