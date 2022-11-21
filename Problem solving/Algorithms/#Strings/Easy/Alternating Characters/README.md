# [Alternating Characters](https://www.hackerrank.com/challenges/alternating-characters)

**Solution**
```python
def alternatingCharacters(s):
    return sum(s[i] == s[i + 1] for i in range(len(s) - 1))
```

**Solution with regex**
```python
from re import sub


def alternatingCharacters(s):
    x = len(s)

    for i in 'AB':
        s = sub(f'({i}){{2,}}', '\1', s)
        
    return x - len(s)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
