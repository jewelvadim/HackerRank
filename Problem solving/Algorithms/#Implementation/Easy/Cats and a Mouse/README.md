# [Cats and a Mouse](https://www.hackerrank.com/challenges/cats-and-a-mouse/problem)

**Solution**
<br>
```python
def catAndMouse(x, y, z):
    a = abs(x-z)
    b = abs(y-z)
    
    result = 'Mouse C'
    
    if a < b:
        result = 'Cat A'
    elif a > b:
        result = 'Cat B'
            
    return result
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
