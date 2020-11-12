#[Plus Minus](https://www.hackerrank.com/challenges/plus-minus/problem)

**Solution**
<br>
```python
def plusMinus(arr):
    result = [0, 0, 0]

    for item in arr:
        if item > 0:
            result[0] += 1
        if item < 0:
            result[1] += 1
        if item == 0:
            result[2] += 1
            
    [print(i / len(arr)) for i in result]
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
