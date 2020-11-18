# [Time Conversion](https://www.hackerrank.com/challenges/time-conversion/problem)

**Solution**
<br>
```python
def timeConversion(s):
    return str(int(s[:2]) % 12 + int(s[-2:] == 'PM') * 12).rjust(2, '0') + s[2:-2]
```

*Explanation*
<br>
If the time is between 12:00 AM and 12:59 AM, we subtract 12 hours. <br>
If the time is between 1:00 AM and 12:59 PM, 24 hour time is same as 12 hour time. <br>
If the time is between 1:00 PM and 11:59 PM, we add 12 hours to input time. <br>

Division mod 12 satisfies the condition AM. Then, if time is PM, add 12. And next, if starts with 0, make it with 2.


If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
