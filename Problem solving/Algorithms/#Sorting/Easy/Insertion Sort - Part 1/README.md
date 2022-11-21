# [Insertion Sort - Part 1](https://www.hackerrank.com/challenges/insertionsort1)

**Solution**
```python
def insertionSort1(n: int, arr: list[int]) -> None:
    n -= 1
    digit = arr[n]
    
    while n:
        
        if arr[n - 1] <= digit:
            break
        
        arr[n] = arr[n - 1]
        n -= 1
            
        print(*arr)            

    arr[n] = digit
    print(*arr)
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
