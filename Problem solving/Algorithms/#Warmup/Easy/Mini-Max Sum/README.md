# [Mini Max Sum](https://www.hackerrank.com/challenges/mini-max-sum/problem)

**First solution**
<br>
*Easy to write, but requires 4 full iterations*
```python
def miniMaxSum(arr):
    sum_ = sum(arr)
    print(sum_ - max(arr), sum_ - min(arr))
```

<br>

**Second solution**
<br>
*Only one iteration*
```python
def miniMaxSum(arr):
    # 1 <= arr[i] <= 10^9
    sum_ = 0
    min_ = 10000000000
    max_ = 0

    for item in arr:
        sum_ += item
        
        if item > max_:
            max_ = item
        
        if item < min_:
            min_ = item
    
    print(sum_ - max_, sum_ - min_)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
