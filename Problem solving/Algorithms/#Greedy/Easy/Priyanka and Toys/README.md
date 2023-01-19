# [Priyanka and Toys](https://www.hackerrank.com/challenges/priyanka-and-toys)

**Solution**
```python
def toys(w: list[int]) -> int:
    result = 0
    
    while w:      
        border = min(w) + 4
        result += 1
        w = [i for i in w if i > border]
            
    return result
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
