# [Super Reduced String](https://www.hackerrank.com/challenges/reduced-string/problem)

**Solution**
```python
def superReducedString(s):
    
    while True:
        letters = set(s)
        flag = len(s)
        
        for letter in letters:
            if letter * 2 in s:
                s = s.replace(letter * 2, '')
        
        if flag == len(s):
            break
        
    return s or 'Empty String'
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
