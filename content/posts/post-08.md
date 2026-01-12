---
title: "学习笔记：算法"
date: 2026-01-08
summary: "记录一次复杂度分析。"
tags: ["算法", "学习"]
---

用最直观的方法理解时间复杂度。

## 代码片段

```python
def two_sum(nums, target):
    seen = {}
    for i, n in enumerate(nums):
        if target - n in seen:
            return [seen[target - n], i]
        seen[n] = i
```

## 图片与链接

![算法](/images/photo-6.png)

相关链接：[LeetCode](https://leetcode.com/)