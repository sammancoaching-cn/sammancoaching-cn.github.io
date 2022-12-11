---
layout: code_smell
title: 沉重的缩进（Heavy Indentation）
source: Emily Bache
---

# 沉重的缩进（Heavy Indentation）

如果同一区块中的所有代码都有相同的缩进程度，大多数代码会更容易阅读，而且如果你要求的话，大多数编辑器会自动用缩进的方式格式化代码。当代码中有许多嵌套的条件和循环时，你会注意到沉重的缩进味道，缩进变得非常深，和/或变化很大。

沉重的缩进是代码的[圈复杂度](https://en.wikipedia.org/wiki/Cyclomatic_complexity)很高的标志，而且代码很难阅读和理解。人类的大脑对于一次能容纳多少复杂的东西是有限制的，大量缩进的代码很可能超出人类的理解能力，因为有太多的东西需要同时记住。