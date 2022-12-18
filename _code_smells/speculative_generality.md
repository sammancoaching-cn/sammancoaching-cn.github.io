---
layout: code_smell
title: 夸夸其谈的通用性（Speculative Generality）
source: Martin Fowler
---

# 夸夸其谈的通用性（Speculative Generality）
额外的代码和钩子以及特殊情况来处理那些（还）不需要的东西。有人认为你会需要这些代码来支持尚未建立的额外功能。通常这些代码已经存在多年，但还没有人需要它。

有时你可以在测试案例中发现这段代码的唯一调用。有时，你的 IDE 能够突出显示不使用的参数以及其他类型的死代码。
