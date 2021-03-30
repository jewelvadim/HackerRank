# [Append and Delete](https://www.hackerrank.com/challenges/append-and-delete/problem)

**Solution**
<br>
```python
def appendAndDelete(s, t, k):
    ls, lt = len(s), len(t)
    amount = ls + lt

    if k >= amount:
        return 'Yes'

    similar = 0
    while similar < min(ls, lt) and s[similar] == t[similar]:
        similar += 1
    amount -= similar * 2

    if similar and k >= amount and (k - amount) % 2 == 0:
        return 'Yes'

    return 'No'
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
