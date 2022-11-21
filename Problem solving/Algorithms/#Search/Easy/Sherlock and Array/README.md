# [Sherlock and Array](https://www.hackerrank.com/challenges/sherlock-and-array)

**Solution**
<br>
```python
def balancedSums(arr: list[int]) -> str:
    left_sum = 0
    right_sum = sum(arr)
    
    for item in arr:
        
        right_sum -= item
        
        if left_sum == right_sum:
            return 'YES'
        
        left_sum += item
    
    return 'NO'
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
