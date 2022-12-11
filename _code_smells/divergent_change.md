---
layout: code_smell
title: 发散式变化（Divergent Change）
source: Martin Fowler
---

# 发散式变化（Divergent Change）
这不是在阅读代码时看到的东西，而是在当你尝试修改代码时发生的事情。当很多不同类型的改变都影响到同一个模块或类时，称之为 "发散式变化（Divergent Change）"。你更希望有一个设计，你可以进去做一个修改，而不需要考虑到附近很多不需要修改的代码。

不过，这种代码坏味道实际上是因为设计问题。发散式变化（Divergent Change）是模块或类不够内聚的标志。

注意：这与[霰弹式修改](shotgun_surgery.html)相似但不同，后者是你的设计有耦合问题的标志。