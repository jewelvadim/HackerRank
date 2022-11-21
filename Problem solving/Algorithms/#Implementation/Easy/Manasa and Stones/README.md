# [Manasa and Stones](https://www.hackerrank.com/challenges/manasa-and-stones)

**Solution**
<br>
```python
def stones(n, a, b):
    return sorted(list(set(a * (n - i - 1) + b * i for i in range(n))))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
