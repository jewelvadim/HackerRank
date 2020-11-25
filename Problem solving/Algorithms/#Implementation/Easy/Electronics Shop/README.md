# [Electronics Shop](https://www.hackerrank.com/challenges/electronics-shop/problem)

**Solution**
<br>
```python
def getMoneySpent(keyboards, drives, b):
    return max([i + j for i in keyboards for j in drives if i + j <= b] + [-1])
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
