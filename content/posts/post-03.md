---
title: "一次代码整理"
date: 2026-01-03
summary: "把重复逻辑抽出为可复用模块。"
tags: ["工程", "代码"]
---

减少偶发 bug 的最好办法，是减少重复。

## 代码片段

```js
export function clamp(n, min, max) {
  return Math.max(min, Math.min(max, n));
}
```

## 图片与链接

![代码](/blog/images/avatar.jpg)

相关链接：[MDN JavaScript](https://developer.mozilla.org/)