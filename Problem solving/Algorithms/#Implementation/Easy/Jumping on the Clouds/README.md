# [Jumping on the Clouds](https://www.hackerrank.com/challenges/jumping-on-the-clouds/problem)

**Solution**
<br>
```python
def jumpingOnClouds(c):
    x = 0
    res = 0
    
    while x < len(c) - 2:
        res += 1 + c[x]
        x += 2 + c[x]
            
    res += x < len(c) - 1
            
    return res
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
