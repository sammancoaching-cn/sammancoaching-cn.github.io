---
layout: code_smell
title: 过长作用域的本地变量（Local Variable with Long Scope）
source: Emily Bache
---

# 作用域长的本地变量（Local Variable with Long Scope）
在[过长函数或方法（Long Function or method）](long_function.html)中，你经常会发现局部变量被用在很长的一段代码中。任何在范围内超过几行的局部变量都会对你的短期记忆造成影响，尤其是当它在多个地方被更新时。

即使是只读变量，如果它们的作用域很长，也会使代码复杂化。仅仅是因为它被用在很多地方就会使你更难从长函数中提取出小的函数或子程序。