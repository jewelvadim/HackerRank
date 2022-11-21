# [Weighted Uniform Strings](https://www.hackerrank.com/challenges/weighted-uniform-string)

**Solution one-liner**
```python
from string import ascii_lowercase
from re import finditer


def weightedUniformStrings(s, queries):
    weights = set()
        
    for el in finditer(r'(\w)\1*', s):
        part = el.group()
        
        weights.update(
            set(
                (
                    (i + 1) * (ascii_lowercase.index(part[0]) + 1) 
                    for i in range(len(part)))
                )
            )
    
    return ('Yes' if q in weights else 'No' for q in queries)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
