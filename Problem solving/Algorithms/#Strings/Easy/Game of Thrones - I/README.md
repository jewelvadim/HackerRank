# [Game of Thrones - I](https://www.hackerrank.com/challenges/game-of-thrones)

**Solution**
```python
def gameOfThrones(s: str) -> str:
    frequency = {symbol: 0 for symbol in set(s)}
    
    for symbol in s:        
        frequency[symbol] ^= 1
            
    return 'YES' if sum(frequency.values()) <= 1 else 'NO'
```
<br>

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
