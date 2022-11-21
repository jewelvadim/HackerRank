# [Plus Minus](https://www.hackerrank.com/challenges/plus-minus)

**Solution**
<br>
```python
def plusMinus(arr):
    result = [0, 0, 0]
    len_ = len(arr)

    for item in arr:
        if item > 0:
            result[0] += 1
        if item < 0:
            result[1] += 1
        if item == 0:
            result[2] += 1
            
    for i in result:
        print(i / len_)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
