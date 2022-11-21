# [Halloween Sale](https://www.hackerrank.com/challenges/halloween-sale)

**Solution**
<br>
```python
def howManyGames(p, d, m, s):
    x = 0
    
    while s >= p:
                
        s -= p
        p = max(p - d, m)
                
        x += 1
            
    return x
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
