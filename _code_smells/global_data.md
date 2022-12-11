---
layout: code_smell
name: global_data
title: 全局数据（Global Data）
source: Martin Fowler
---

# 全局数据（Global Data）
可以从代码库的任何地方修改数据。这很难推理，也很难进行单元测试。如果你不能轻易地找到所有改变全局数据的代码片段，那就更糟糕了。单例（Singleton）是全局的一种，类变量也是如此。你能保证在程序开始后保持不变的全局数据问题不大。