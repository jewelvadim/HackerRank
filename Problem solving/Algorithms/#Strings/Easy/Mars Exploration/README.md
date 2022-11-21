# [Mars Exploration](https://www.hackerrank.com/challenges/mars-exploration)

**Solution**
```python
def marsExploration(s):
    return sum([(k % 3 != 1 and v != 'S') or (k % 3 == 1 and v != 'O') for k, v in enumerate(s)])
```

<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
