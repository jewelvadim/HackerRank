# [Strange Counter](https://www.hackerrank.com/challenges/strange-code/problem)

**Solution**
<br>
```python
def strangeCounter(t):
    i = 3
    start = 1
    
    while start <= t:
        start += i
        i *= 2
        
    return start - t
```
<br>

**One-liner with math**
<br>
```python
def strangeCounter(t):
    return 3 * (2 ** math.ceil(math.log2(1 + t / 3)) - 1) - t + 1
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
