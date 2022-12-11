---
layout: code_smell
title: 重复的 Switch（Repeated Switches）
source: Martin Fowler
---

# 重复的 Switch（Repeated Switches）
如果你在几个地方看到相同的 "switch" 语句，这说明你可以使用更灵活的动态结构，比如多态性。一个 switch 语句本身也许并不太危险，但如果你有几个，那么就是恼人的重复。如果你在一个 switch 语句中添加一个新的子句，你可能要记得更新所有的子句。

