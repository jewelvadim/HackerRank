# [Pangrams](https://www.hackerrank.com/challenges/pangrams)

**Solution**
```python
from string import ascii_lowercase


def pangrams(s):
    return 'not ' * any([i not in s.lower() for i in ascii_lowercase]) + 'pangram'
```

<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
