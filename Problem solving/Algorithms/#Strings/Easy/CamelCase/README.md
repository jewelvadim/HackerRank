# [CamelCase](https://www.hackerrank.com/challenges/camelcase/problem)

**Solution**
```python
import re

def camelcase(s):
    return len(re.findall(r'[A-Z]', s)) + 1
```

**Solution without dependencies**
```python
def camelcase(s):
    return sum([i.isupper() for i in s]) + 1
```
<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
