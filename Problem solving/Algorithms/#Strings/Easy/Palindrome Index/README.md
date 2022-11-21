# [Palindrome Index](https://www.hackerrank.com/challenges/palindrome-index)

**Solution**
```python
def palindromeIndex(s):
    
    if s != s[::-1]:
        n = len(s)
        
        for k in range((n + 1) // 2):
            
            if s[k] != s[n - k - 1]:
                
                temp = s[k + 1:n - k]
                
                if temp == temp[::-1]:
                    return k
                
                temp = s[k:n - k - 1]
                
                if temp == temp[::-1]:
                    return n - k - 1

    return -1
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
