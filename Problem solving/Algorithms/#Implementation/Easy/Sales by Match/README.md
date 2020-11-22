# [Sales by Match](https://www.hackerrank.com/challenges/sock-merchant/problem)

**Solution in one iteration**
<br>
```python
def sockMerchant(n, ar):
    result = 0
    dict_ = {}
    
    for i in ar:
        if i not in dict_:
            dict_[i] = 1
        elif dict_[i]:
            dict_[i] -= 1
            result += 1
        else:
            dict_[i] += 1
            
    return result
```


**Solution in one string O(n^2)**
<br>
```python
def sockMerchant(n, ar):
    return sum([ar.count(x) // 2 for x in set(ar)])
```


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
