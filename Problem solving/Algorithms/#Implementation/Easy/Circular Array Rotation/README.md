# [Circular Array Rotation](https://www.hackerrank.com/challenges/circular-array-rotation/problem)

**Solution**
<br>
```python
def circularArrayRotation(a, k, queries):            
    return [a[i - k % len(a)] for i in queries]
```
*Explanation*
<br>
New value is old value + shift. Just calc old value.
<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
