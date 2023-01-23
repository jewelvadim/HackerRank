# [Grid Challenge](https://www.hackerrank.com/challenges/grid-challenge)

**Solution**
```python
def gridChallenge(grid: list[str]) -> str:
    n = len(grid)
    m = len(grid[0])
    grid[0] = sorted(grid[0])
    
    for i in range(1, n):
        grid[i] = sorted(grid[i])
    
        for j in range(m):
            if grid[i][j] < grid[i - 1][j]:
                return 'NO'
    
    return 'YES'
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
