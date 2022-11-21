# [Sequence Equation](https://www.hackerrank.com/challenges/permutation-equation)

**Solution**
<br>
```python
def permutationEquation(p):
    return [p.index(p.index(i+1)+1)+1 for i in range(len(p))]
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
