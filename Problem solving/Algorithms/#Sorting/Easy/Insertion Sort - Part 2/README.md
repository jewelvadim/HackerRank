# [Insertion Sort - Part 2](https://www.hackerrank.com/challenges/insertionsort2)

**Solution**
```python
def insertionSort2(n: int, arr: list[int]) -> None:
    
    for i in range(1, n):
        current_index = i
        current_value = arr[i]
                
        while current_index and arr[current_index - 1] > current_value:
            arr[current_index] = arr[current_index - 1]
            
            current_index -= 1
            
        arr[current_index] = current_value
        
        print(*arr)
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
