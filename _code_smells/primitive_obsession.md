---
layout: code_smell
name: primitive_obsession
title: 基本类型偏执（Primitive Obsession）
source: Martin Fowler
---

# 基本类型偏执（Primitive Obsession）
当你使用普通的内置原始类型，如 `string`，`int`，`float` 等。这可能是一个信号，你应该有类来表示领域概念，如货币、坐标、范围、电话号码等。如果你使用原始类型，你就有可能犯错误，比如把英寸加到厘米上，或者不能一致地显示有或没有国际代码的电话号码。