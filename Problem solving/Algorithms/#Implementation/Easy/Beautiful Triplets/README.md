# [Beautiful Triplets](https://www.hackerrank.com/challenges/beautiful-triplets)

**One string solution (just for fun)**
<br>
```python
def beautifulTriplets(d, arr):
    res = 0
    
    for i in arr:
        j = i + d
        k = j + d
        
        res += j in arr and k in arr and arr.index(k) > arr.index(j) > arr.index(i)
    
    return res
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
