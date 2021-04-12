# [ACM ICPC Team](https://www.hackerrank.com/challenges/acm-icpc-team/problem)

**Solution**
<br>
```python
def acmTeam(topic):
    topic = list(map(int, topic))
    n = len(topic)
    
    max_ = 0
    max_count = 0
    
    for i in range(n):
        for j in range(i + 1, n):
            
            s = sum(k != '0' for k in str(topic[i] + topic[j]))
        
            if s > max_:
                max_ = s
                max_count = 1
            elif s == max_:
                max_count += 1
    
    return max_, max_count
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
