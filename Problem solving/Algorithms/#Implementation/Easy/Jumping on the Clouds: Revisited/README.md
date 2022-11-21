# [Jumping on the Clouds: Revisited](https://www.hackerrank.com/challenges/jumping-on-the-clouds-revisited)

**Solution**
<br>
```python
def jumpingOnClouds(c, k):

    e = 100    
    position = 0
    n = len(c)
    
    while True:
        position = (position + k) % n
        e -= 1 + 2 * c[position]
        
        if position == 0:
            break

    return e
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
