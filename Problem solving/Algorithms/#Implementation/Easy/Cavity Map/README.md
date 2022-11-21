# [README.md](https://www.hackerrank.com/challenges/cavity-map)

**Solution**
<br>
```python
def cavityMap(grid):
    
    if len(grid) > 2:
        for i in range(1, len(grid) - 1):
            grid[i] = list(grid[i])
                                    
            for j in range(1, len(grid[i])- 1):
                points = [grid[i-1][j], grid[i+1][j], grid[i][j-1], grid[i][j+1]]
                
                if all([grid[i][j] > x for x in points]):
                    grid[i][j] = 'X'
            
            grid[i] = ''.join(grid[i])
            
    return grid
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
