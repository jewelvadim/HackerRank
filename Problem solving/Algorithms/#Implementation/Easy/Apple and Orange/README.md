# [Apple and Orange](https://www.hackerrank.com/challenges/apple-and-orange)

**Solution**
<br>
```python
def countApplesAndOranges(s, t, a, b, apples, oranges):
    print(sum((s <= x + a <= t for x in apples)))
    print(sum((s <= x + b <= t for x in oranges)))
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
