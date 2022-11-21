# [Viral Advertising](https://www.hackerrank.com/challenges/strange-advertising)

**Solution**
<br>
```python
def viralAdvertising(n):
    s = 5
    result = 0
    
    for _ in range(n):
        s = s // 2 * 3
        result += s
    
    return result // 3
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
