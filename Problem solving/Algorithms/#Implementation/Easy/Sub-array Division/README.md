# [Sub-array Division](https://www.hackerrank.com/challenges/the-birthday-bar)

**Solution**
<br>
```python
def birthday(s, d, m):
    return sum((sum(s[i:i+m]) == d for i in range(len(s) - m + 1)))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
