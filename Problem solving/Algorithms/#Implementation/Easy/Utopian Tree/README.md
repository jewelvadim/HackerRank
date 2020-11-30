# [Utopian Tree](https://www.hackerrank.com/challenges/utopian-tree/problem)

**Solution**
<br>
```python
def utopianTree(n):
    result = 1
    
    for _ in range(n // 2):
        result = 2 * result + 1
        
    return 2 * result if n % 2 else result
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
