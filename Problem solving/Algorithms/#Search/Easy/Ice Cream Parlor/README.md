# [Ice Cream Parlor](https://www.hackerrank.com/challenges/icecream-parlor)

**Solution**
<br>
```python
def icecreamParlor(m: int, arr: list[int]) -> tuple[int, int]:
    for i in range(len(arr)):
        try:
            j = arr.index(m - arr[i], i + 1)
        except ValueError:
            continue
        else:
            return i + 1, j + 1
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
