#[Staircase](https://www.hackerrank.com/challenges/staircase/problem)

This is the task from [HackerRank](https://www.hackerrank.com/dashboard)
<br>
<br>

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

<br>
If it useful for you - I am happy. <br>
If you know, how to make my solution better - please, text me.
