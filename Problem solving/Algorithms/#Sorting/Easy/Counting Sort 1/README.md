# [Counting Sort 1](https://www.hackerrank.com/challenges/countingsort1/problem)

**Solution**
```python
def countingSort(arr: list[int]) -> list[int]:
    result = [0] * 100
    
    for i in arr:
        result[i] += 1
        
    return result
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
