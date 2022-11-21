# [Quicksort 1 - Partition](https://www.hackerrank.com/challenges/quicksort1)

**Solution**
```python
def quickSort(arr: list[int]) -> list[int]:
    left = []
    right = []
    equal = []
    basis = arr[0]
    
    for i in arr:
        if i < basis:
            left.append(i)
        elif i > basis:
            right.append(i)
        else:
            equal.append(i)
            
    return left + equal + right
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
