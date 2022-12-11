---
layout: code_smell
title: 被拒绝的遗赠（Refused Bequest）
source: Martin Fowler
wikipedia_source: true
---

# 被拒绝的遗赠（Refused Bequest）
当一个子类从其父类那里继承了方法和字段，但却不需要它们。这往往是子类不能替代其父类的标志。在这种情况下，它就违反了里氏替换原则（Liskov Substitution principle）。

