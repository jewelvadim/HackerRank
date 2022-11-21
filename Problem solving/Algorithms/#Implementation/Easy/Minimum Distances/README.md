# [Minimum Distances](https://www.hackerrank.com/challenges/minimum-distances)

**Solution**
<br>
```python
def minimumDistances(a):
    reversed_a = a[::-1]
    n = len(a)
    
    return min(list(filter(lambda x: x, (n - 1 - reversed_a.index(i) - a.index(i) for i in set(a)))) or [-1])
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
