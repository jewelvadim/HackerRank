# [Permuting Two Arrays](https://www.hackerrank.com/challenges/two-arrays)

**Solution**
```python
def twoArrays(k, A, B):
    return 'YES' if all(a + b >= k for a, b in zip(sorted(A), sorted(B, reverse=True))) else 'NO'
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
