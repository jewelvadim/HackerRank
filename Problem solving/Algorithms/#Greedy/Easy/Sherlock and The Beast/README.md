# [Sherlock and The Beast](https://www.hackerrank.com/challenges/sherlock-and-the-beast)

**Solution**
```python
def decentNumber(n: int) -> None:
    
    for i in range(n + 1):
        thirds = i
        fives = n - thirds
        
        if fives % 3 == 0 and thirds % 5 == 0:
            print('5' * fives + '3' * thirds)
            break

    else:
        print('-1')
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
