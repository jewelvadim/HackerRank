# [Utopian Tree](https://www.hackerrank.com/challenges/utopian-tree/problem)

**Solution**
<br>
```python
def utopianTree(n):
    result = 1
    
    for _ in range(n // 2):
        result = 2 * result + 1
        
    return 2 * result if n % 2 else result
```
<br>
<br>

**Solution with ```<<``` operand**
<br>
```python
def utopianTree(n):
    return ~ (~ 1 << (n >> 1)) << n % 2
```
*Explanation*
<br>
x << y = x * 2**y
~ x = - (x + 1)
<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
