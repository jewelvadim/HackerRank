# [Closest Numbers](https://www.hackerrank.com/challenges/closest-numbers)

**Solution**
```python
def closestNumbers(arr: list[int]) -> list[int]:
    arr.sort()
    
    minimum = arr[1] - arr[0]
    result = arr[0:2]

    for i in range(1, len(arr) - 1):
        difference = arr[i + 1] - arr[i]
        
        if difference < minimum:
            minimum = difference
            result = arr[i:i + 2]
            
        elif difference == minimum:
            result += arr[i:i + 2]
    
    return result
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
