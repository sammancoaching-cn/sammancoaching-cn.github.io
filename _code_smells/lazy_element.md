---
layout: code_smell
name: lazy_element
title: 冗赘的元素（Lazy Element）
source: Martin Fowler
---

# 冗赘的元素（Lazy Element）
不需要的结构，可以很容易地被内联而不损失任何重要的东西。例如，一个函数的名字和它的正文中的代码是一样的。有时，懒惰元素的出现是重构的结果--功能被移到了其他地方，剩下的东西不再有价值了。有时它是由于[夸夸其谈的通用性（Speculative Generality）](speculative_generality.html)而产生的，你现在意识到它将永远不会被需要。