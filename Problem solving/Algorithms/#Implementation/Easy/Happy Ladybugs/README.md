# [Happy Ladybugs](https://www.hackerrank.com/challenges/happy-ladybugs/problem)

**Solution**
<br>
```python
def happyLadybugs(b):
    for i in set(b):
        if b.count(i) == 1 and i != '_':
            return 'NO'
    
    if '_' not in set(b):
        for i in range(len(b) - 1):
            if b[i] != b[i+1] and (i == 0 or b[i-1] != b[i]):
                return 'NO'
        
    return 'YES'
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
