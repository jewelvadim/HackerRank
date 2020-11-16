#[Between Two Sets](https://www.hackerrank.com/challenges/between-two-sets/problem)

**One string solution (just for fun)**
<br>
```python
def getTotalX(a, b):
    return sum((all((i % x == 0 for x in a)) and all((x % i == 0 for x in b)) for i in range(max(a), min(b) + 1)))
```

*P.S.*
<br>
It is more correct to use lcm and gcd as left and right borders of range, but my values are enough for conditions of this problem.

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
