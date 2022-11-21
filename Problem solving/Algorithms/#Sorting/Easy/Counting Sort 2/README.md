# [Counting Sort 2](https://www.hackerrank.com/challenges/countingsort2)

**Solution**
```python
def countingSort(arr: list[int]) -> list[int]:
    frequency = [0] * 100
    result = []
    
    for i in arr:
        frequency[i] += 1
        
    for i, v in enumerate(frequency):
        if v:
            result += [i] * v
            
    return result
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
