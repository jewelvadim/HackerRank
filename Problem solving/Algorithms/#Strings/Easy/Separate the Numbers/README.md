# [Separate the Numbers](https://www.hackerrank.com/challenges/separate-the-numbers/problem)

**Solution**
```python
def separateNumbers(s):
    current_len = 1
    
    while current_len <= len(s) // 2:
        str_ = s[:current_len]
        num_ = int(str_)
        min_ = num_
        
        while s.startswith(str_) and s != str_:
            num_ += 1
            str_ += str(num_)
                    
        if str_ == s:
            print('YES', min_)    
            break
            
        current_len += 1
        
    else:
        print('NO')  
```

<br>

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
