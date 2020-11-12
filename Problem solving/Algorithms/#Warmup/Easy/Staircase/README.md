#[Staircase](https://www.hackerrank.com/challenges/staircase)

**First solution**
<br>
*simple*
<br>
```python
def staircase(n):
    [print(' ' * (n-i) + i * '#') for i in range(1, n+1)]
```

<br>

**Second solution**
<br>
*with python rjust*
<br>
```python
def staircase(n):        
    [print(str('#' * i).rjust(n)) for i in range(1, n+1)]
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
