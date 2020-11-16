#[Grading Students](https://www.hackerrank.com/challenges/grading/problem)

**Solution**
<br>
```python
def gradingStudents(grades):
    return (i + 5 - i % 5 if i > 37 and i % 5 > 2 else i for i in grades)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
