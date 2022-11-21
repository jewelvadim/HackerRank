# [Funny String](https://www.hackerrank.com/challenges/funny-string)

**Solution**
```python
def funnyString(s):
    x = [abs(ord(s[i+1]) - ord(s[i])) for i in range(len(s) - 1)]
    return 'Not ' * (x != x[::-1]) + 'Funny'
```

<br>

**Solution 2**
```python
def funnyString(s):
    
    for i in range(len(s) // 2):
        if abs(ord(s[i]) - ord(s[i + 1])) != abs(ord(s[len(s) - 1 - i]) - ord(s[len(s) - 2 - i])):
            return 'Not Funny'
    
    return 'Funny'
```

<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
