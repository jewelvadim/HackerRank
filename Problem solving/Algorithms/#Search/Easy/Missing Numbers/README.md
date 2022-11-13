# [Missing Numbers](https://www.hackerrank.com/challenges/missing-numbers/problem)

**Solution**
<br>
```python
def missingNumbers(arr: list[int], brr: list[int]) -> list[int]:
    d = {}
    
    for item in arr:
        if item in d:
            d[item] -= 1
        else:
            d[item] = -1
            
    for item in brr:
        if item in d:
            d[item] += 1
        else:
            d[item] = 1
            
    return sorted(item for item in d if d[item] > 0)

```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
