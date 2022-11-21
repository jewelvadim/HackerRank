# [Modified Kaprekar Numbers](https://www.hackerrank.com/challenges/kaprekar-numbers)

**Solution**
<br>
```python
def kaprekarNumbers(p, q):
    res = []
    
    for i in range(p, q + 1):
        x = i ** 2
        d = 10 ** len(str(i))
                
        if x // d + x % d == i:
            res.append(i)
            
    if res:
        print(*res)
    else:
        print('INVALID RANGE')
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
