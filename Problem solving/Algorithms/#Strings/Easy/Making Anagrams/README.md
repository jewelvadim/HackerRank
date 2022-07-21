# [Making Anagrams](https://www.hackerrank.com/challenges/making-anagrams/problem)

**Solution**
```python
def makingAnagrams(s1: str, s2: str) -> int:
    d = {}
    
    for s in s1:
        d[s] = d.get(s, 0) + 1

    for s in s2:
        d[s] = d.get(s, 0) - 1

    return sum(abs(s) for s in d.values())
```

<br>

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
