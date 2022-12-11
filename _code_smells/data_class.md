---
layout: code_smell
title: 纯数据类（Data Class）
source: Martin Fowler
---

# 纯数据类（Data Class）
这种类有字段，即可变的状态，但没有其他行为。这些字段可能有获取和设置的方法，也可能是公共的。在其他地方可能有对这些数据进行操作的函数，这些函数可以移到这里，使之成为一个更面向对象的设计。