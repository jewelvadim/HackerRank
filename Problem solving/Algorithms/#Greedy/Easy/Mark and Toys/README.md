# [Mark and Toys](https://www.hackerrank.com/challenges/mark-and-toys)

**Solution**
```python
def maximumToys(prices: list[int], k: int) -> int:
    for i, v in enumerate(sorted(prices)):
        k -= v
        
        if k <= 0:
            return i
    
    return len(prices)
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
