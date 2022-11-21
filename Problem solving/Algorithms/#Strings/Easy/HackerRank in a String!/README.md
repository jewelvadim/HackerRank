# [HackerRank in a String!](https://www.hackerrank.com/challenges/hackerrank-in-a-string)

**Solution**
```python
def hackerrankInString(s):
    x = list('hackerrank')
    
    for i in s:
        if i == x[0]:
            x.pop(0)
            
            if not x:
                return 'YES'
    
    return 'NO'
```

<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
