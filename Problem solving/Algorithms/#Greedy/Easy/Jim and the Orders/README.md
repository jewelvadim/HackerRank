# [Jim and the Orders](https://www.hackerrank.com/challenges/jim-and-the-orders)

**Solution**
```python
def jimOrders(orders: list[list[int]]) -> list[int]:
    result = {i + 1: sum(v) for i, v in enumerate(orders)}
    
    return sorted(result, key=lambda x: (result[x], x))
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
