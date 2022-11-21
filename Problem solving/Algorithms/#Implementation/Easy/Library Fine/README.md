# [Library Fine](https://www.hackerrank.com/challenges/library-fine)

**Solution**
<br>
```python
def libraryFine(d1, m1, y1, d2, m2, y2):    
    if y1 > y2:
        return 10000
    elif y1 == y2 and m1 > m2:
        return 500 * (m1 - m2)
    elif y1 == y2 and m1 == m2 and d1 > d2:
        return 15 * (d1 - d2)
    else:
        return 0
```

**One-liner**
<br>
```python
def libraryFine(d1, m1, y1, d2, m2, y2):
    return (y1 > y2) * 10000 + (y1 == y2 and m1 > m2) * 500 * (m1 - m2) + (y1 == y2 and m1 == m2 and d1 > d2) * 15 * (d1 - d2)
```


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
