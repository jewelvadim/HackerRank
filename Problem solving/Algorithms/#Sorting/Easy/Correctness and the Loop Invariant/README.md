# [Correctness and the Loop Invariant](https://www.hackerrank.com/challenges/correctness-invariant)

**Solution**
```python
def insertion_sort(l: list[int]) -> None:
    for i in range(1, len(l)):
        j = i - 1
        key = l[i]
        
        while (j >= 0) and (l[j] > key):
           l[j + 1] = l[j]
           j -= 1
        
        l[j + 1] = key
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
