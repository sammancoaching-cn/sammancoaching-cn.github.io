---
layout: code_smell
title: 中间人（Middle Man）
source: Martin Fowler
---

# 中间人（Middle Man）
一个类除了将所有的调用转发到另一个类之外没有做更多的事情，它自己的行为很少或没有。这可能是一个信号，这个类的客户应该直接与所有被转发的调用的类对话。