# [Divisible Sum Pairs](https://www.hackerrank.com/challenges/divisible-sum-pairs/problem)

**Solution**
<br>
```python
def divisibleSumPairs(n, k, ar):
    return sum((ar[i] + ar[j]) % k == 0 for i in range(n-1) for j in range(i+1, n))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
