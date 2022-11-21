# [The Love-Letter Mystery](https://www.hackerrank.com/challenges/the-love-letter-mystery)

**Solution**
```python
def theLoveLetterMystery(s):
    return sum(ord(l[1]) - ord(l[0]) for l in zip(s, s[::-1]) if l[1] > l[0])
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
