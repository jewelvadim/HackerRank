# [Minimum Absolute Difference in an Array](https://www.hackerrank.com/challenges/minimum-absolute-difference-in-an-array)

**Solution**
```python
from math import inf


def minimumAbsoluteDifference(arr: list[int]) -> int:
    arr.sort()
    n = len(arr)

    if n == len(set(arr)):
        result = inf

        for i in range(n - 1):
            abs_difference = abs(arr[i] - arr[i + 1])

            if abs_difference < result:
                result = abs_difference
    else:
        result = 0

    return result

```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
