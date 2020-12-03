# [Beautiful Days at the Movies](https://www.hackerrank.com/challenges/beautiful-days-at-the-movies/problem)

**Solution**
<br>
```python
def beautifulDays(i, j, k):
    return sum((abs(x - int(str(x)[::-1])) % k == 0 for x in range(i, j+1)))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
