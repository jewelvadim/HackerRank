# [Fair Rations](https://www.hackerrank.com/challenges/fair-rations)

**Solution**
<br>
```python
def fairRations(B):
    res = 0
    
    for i in range(len(B) - 1):
        b = B[i] % 2
        B[i] += b
        B[i+1] += b
        res += b
        
    if B[-1] % 2:
        return 'NO'
    else:
        return str(res * 2)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
