# [Birthday Cake Candles](https://www.hackerrank.com/challenges/birthday-cake-candles)

**First solution**
<br>
*With using Counter from collections*
```python
from collections import Counter

def birthdayCakeCandles(candles):    
    return Counter(candles).most_common(1)[0][1]
```

<br>

**Second solution**
<br>
*Only one iteration*
```python
def birthdayCakeCandles(candles):    
    max_ = 0
    result = 0
    
    for item in candles:
        if item == max_:
            result += 1
        elif item > max_:
            max_ = item
            result = 1
            
    return result
```

<br>

**Third solution**
<br>
*Extremly simple*
```python
def birthdayCakeCandles(candles):    
    return candles.count(max(candles))
```


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
