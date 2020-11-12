#[Number Line Jumps](https://www.hackerrank.com/challenges/kangaroo/problem)

**Solution**
<br>
```python
def kangaroo(x1, v1, x2, v2):
    # this solution is correct because x1 != x2 based on problem conditions
    result = 'NO'
    
    if v1 != v2:
        y = (x2 - x1) / (v1 - v2)
    
        if y.is_integer() and y >= 0:
            result = 'YES'
    
    return result
```
*Explanation*
<br>
You need to find intersection point of two linear equations: v1 * x + x1 = v2 * x + x2 
<br>
<br>

**Solution in one string (just for fun)**
<br>
```python
def kangaroo(x1, v1, x2, v2):
    return 'YES' if v1 != v2 and (x2 - x1) / (v1 - v2) >= 0 and (x2 - x1) % (v1 - v2) == 0 else 'NO'
```


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
