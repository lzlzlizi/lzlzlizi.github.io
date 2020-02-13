---
title: trickypython
date: 2020-02-13 14:30:04
tags: python
---

# Some tricky problems

## initialize a 2-D list

```python
nums = [1,4,65]
L = len(nums)
DP = [[0] * L] * L
for i in  range(len(DP)):
    DP[i][i] = nums[i]
    print(DP,nums[i], DP[i][i])
```

```
[[1, 0, 0], [1, 0, 0], [1, 0, 0]] 1 1
[[1, 4, 0], [1, 4, 0], [1, 4, 0]] 4 4
[[1, 4, 65], [1, 4, 65], [1, 4, 65]] 65 65
```

It seems  like the 2-D array is actually sharing the same raw.

Therefore, one should using  ```DP = [[0 for _ in nums] for _ in nums]```.