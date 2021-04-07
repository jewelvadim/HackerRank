# [Day of the Programmer](https://www.hackerrank.com/challenges/day-of-the-programmer/problem)

**Solution**
<br>
```python
def dayOfProgrammer(year):
    day_ = 13
    
    if year == 1918:
        day_ = 26
    elif (year < 1918 and year % 4 == 0) or (year > 1918 and (year % 400 == 0 or (year % 4 == 0 and year % 100 != 0))):
        day_ = 12
            
    return '{}.09.{}'.format(day_, year)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
