# [Strong Password](https://www.hackerrank.com/challenges/strong-password)

**Solution**
```python
def minimumNumber(n, password):
    add = 4
    add -= any([i.isdigit() for i in password])
    add -= any([i.isupper() for i in password])
    add -= any([i.islower() for i in password])
    add -= any([i in '!@#$%^&*()-+' for i in password])

    return max(add, 6 - n)
```

**Solution with regexp**
```python
import re


def minimumNumber(n, password):
    add = 4 - sum(
        bool(re.search(i, password)) 
        for i in [r'[a-z]', r'[A-Z]', r'[0-9]', r'[\!\@\#\$\%\^\&\*\(\)\-\+]']
    )
    
    return max(add, 6 - n)
```
<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
