# [Repeated String](https://www.hackerrank.com/challenges/repeated-string)

**Solution**
<br>
```python
def repeatedString(s, n):
    return s.count('a') * (n // len(s)) + s[:n % len(s)].count('a')
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
