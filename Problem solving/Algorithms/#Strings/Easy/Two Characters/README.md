# [Two Characters](https://www.hackerrank.com/challenges/two-characters)

**Solution one-liner**
```python
from itertools import combinations


def alternate(s):
    return max(
        list(
            map(
                len,
                filter(
                    lambda t: len(set(t[::2])) == len(set(t[1::2])) == 1,
                    [list(filter(lambda x: x in i, s)) for i in combinations(set(s), 2)]
                )
            )
        ) + [0]
    )
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
