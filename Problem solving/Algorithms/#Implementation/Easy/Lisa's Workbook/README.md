# [Lisa's Workbook](https://www.hackerrank.com/challenges/lisa-workbook/problem)

**Solution**
<br>
```python
def workbook(n, k, arr):
    start = 0
    res = 0

    for i in arr:
        res += sum(j == start + j // k + bool(j % k) for j in range(start + 1, i + 1))
        start += i // k + bool(i % k)
                
    return res
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
