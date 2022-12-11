---
layout: code_smell
name: long_function
title: 过长函数（Long Function）
source: Martin Fowler
wikipedia_source: true
---

# 过长函数 和 过长方法（Long Function and Long Method）
如果函数太长，那么它往往难以阅读和理解。在现代编译器中，将部分内容分解成子程序对性能影响不大。如果这些子程序或私有函数命名的很好，那么它将使原始函数更容易阅读。解释代码块的 [注释（comment）](comment.html) 的存在就是一个提示，表明你会很好地引入一个私有函数。
