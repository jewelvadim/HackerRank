# [Counting Valleys](https://www.hackerrank.com/challenges/counting-valleys)

**Solution**
<br>
```python
def countingValleys(steps, path):
    result = stage = 0
    
    for step in range(steps):
        if path[step] == 'U':
            stage += 1
            
            if stage == 0:
                result += 1
            
        else:
            stage -= 1
            
    return result
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
