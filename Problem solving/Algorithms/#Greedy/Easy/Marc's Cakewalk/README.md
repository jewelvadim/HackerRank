# [Marc's Cakewalk](https://www.hackerrank.com/challenges/marcs-cakewalk)

**Solution**
```python
def marcsCakewalk(calorie: list[int]) -> int:
    return sum(val * 2 ** idx for idx, val in enumerate(sorted(calorie, reverse=True)))
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
