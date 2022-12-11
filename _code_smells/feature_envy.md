---
layout: code_smell
name: feature_envy
title: 依恋情结（Feature Envy）
source: Martin Fowler
wikipedia_source: true
---

# 依恋情结（Feature Envy）
当一个类或模块中的函数大量使用另一个类或模块中的函数和/或数据，以至于它可能属于那里。通常在面向对象的设计中，你希望函数与它们所处理的数据生活在同一个类上。把一起变化的东西放在一起。
