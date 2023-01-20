# [Maximum Perimeter Triangle](https://www.hackerrank.com/challenges/maximum-perimeter-triangle)

**Solution**
```python
from functools import lru_cache
from itertools import combinations


@lru_cache
def is_non_degenerate(a: int, b: int, c: int) -> bool:
    return a + b > c and a + c > b and b + c > a

    
def maximumPerimeterTriangle(sticks: list[int]) -> list[int]:
    max_triangle = None
    
    for triangle in combinations(sticks, 3):
        if is_non_degenerate(*triangle):
            
            if max_triangle is None:
                max_triangle = triangle
                
            elif sum(triangle) > sum(max_triangle):
                max_triangle = triangle
                
            elif sum(triangle) == sum(max_triangle):
                
                if max(triangle) > max(max_triangle):
                    max_triangle = triangle
                
                elif max(triangle) == max(max_triangle) and min(triangle) > min(max_triangle):
                    max_triangle = triangle
                    
    return sorted(max_triangle or [-1])
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
