# [Caesar Cipher](https://www.hackerrank.com/challenges/caesar-cipher-1)

**Solution**
```python
def caesarCipher(s, k):
    alphabet = 'abcdefghijklmnopqrstuvwxyz'
    result = []
    
    for symbol in s:
        if symbol.isalpha():
            
            is_upper = symbol.isupper()
            
            new_symbol = alphabet[(alphabet.index(symbol.lower()) + k) % len(alphabet)]
            
            if is_upper:
                new_symbol = new_symbol.upper()
            
            result.append(new_symbol)
        else:
            result.append(symbol)
    
    return ''.join(result)
```

**Solution one-liner**
```python
from string import ascii_lowercase as al, ascii_uppercase as au


def caesarCipher(s, k):
    n = len(al)

    return ''.join(
        map(
            lambda x: x if not x.isalpha() else au[(au.index(x) + k) % n] if x.isupper() else al[(al.index(x) + k) % n],
            s
        )
    )
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
