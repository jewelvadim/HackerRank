# [Luck Balance](https://www.hackerrank.com/challenges/luck-balance)

**Solution**
```python
def luckBalance(k: int, contests: list[list[int]]) -> int:
    luck = 0
    important_tests_luck = []

    for luck_amount, is_important in contests:
        if is_important:
            for i, v in enumerate(important_tests_luck):
                if v <= luck_amount:
                    important_tests_luck.insert(i, luck_amount)
                    break
            else:
                important_tests_luck.append(luck_amount)

        else:
            luck += luck_amount

    return luck + sum(important_tests_luck[:k]) - sum(important_tests_luck[k:])
```

If it is useful for you - I am happy. Please, press **star**.  
If you know, how to make my solution better - please, text me.
