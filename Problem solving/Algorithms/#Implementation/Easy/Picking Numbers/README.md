# [Picking Numbers](https://www.hackerrank.com/challenges/picking-numbers)

**Solution**
<br>
```python
def pickingNumbers(a):
    return max((a.count(i) + a.count(i + 1) for i in set(a)))    
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
