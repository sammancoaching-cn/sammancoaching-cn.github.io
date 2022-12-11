---
layout: code_smell
title: 临时字段（Temporary Field）
source: Martin Fowler
---

# 临时字段（Temporary Field）
一个类有一个字段，它只在特定情况下被设置。在其他时候，它可能是空的或空的。这可能是一个信号，你应该把这个字段移到另一个类中，在那里它将一直被设置。同时也要移动任何使用这个字段的函数。