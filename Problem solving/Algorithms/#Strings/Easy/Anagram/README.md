# [Anagram](https://www.hackerrank.com/challenges/anagram/problem)

**Solution**
```python
def anagram(s: str) -> int:
    result = -1
    n = len(s)
    
    if n % 2 == 0:
        frequency = {}
        
        for symbol in s[:n // 2]:
            frequency[symbol] = frequency.get(symbol, 0) + 1
            
        for symbol in s[n // 2:]:
            frequency[symbol] = frequency.get(symbol, 0) - 1
            
        result = sum(filter(lambda x: x > 0, frequency.values()))
    
    return result
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
