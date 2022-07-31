# [Running Time of Algorithms](https://www.hackerrank.com/challenges/runningtime/problem)

**Solution**
```python
def runningTime(arr: list[int]) -> int:
    k = 0
    
    for i in range(1, len(arr)):
        current_index = i
        current_value = arr[i]
        
        while current_index and arr[current_index - 1] > current_value:
            arr[current_index] = arr[current_index - 1]
            current_index -= 1
            k += 1
            
        arr[current_index] = current_value

    return k
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
