# [Find Digits](https://www.hackerrank.com/challenges/find-digits/problem)

**Solution**
<br>
```python
def findDigits(n):
    return sum(n % int(i) == 0 for i in str(n) if i != '0')
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
