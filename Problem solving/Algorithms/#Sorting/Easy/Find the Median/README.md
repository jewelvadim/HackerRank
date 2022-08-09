# [Find the Median](https://www.hackerrank.com/challenges/find-the-median/problem)

**Solution O(n^2)**
```python
def findMedian(arr: list[int]) -> int:
    arr.sort()
    return arr[len(arr) // 2]
```

**Solution O(n*log(n))**  
The idea of the solution is to use https://en.wikipedia.org/wiki/Quickselect
```python
def quickselect(array: list[int], index: int, pivot: int) -> int:
    left = []
    right = []
    pivots = 0
    
    for i in array:
        if i < pivot:
            left.append(i)
        elif i > pivot:
            right.append(i)
        else:
            pivots += 1
        
    if len(left) > index:
        pivot = left[0]
        array = left
        
    elif len(left) + pivots > index:
        return pivot
    
    else:
        pivot = right[0]
        index -= len(left) + pivots
        array = right
        
    return quickselect(array, index, pivot)

def findMedian(arr: list[int]) -> int:
    index = len(arr) // 2
    pivot = arr[0]
    
    return quickselect(arr, index, pivot)
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
