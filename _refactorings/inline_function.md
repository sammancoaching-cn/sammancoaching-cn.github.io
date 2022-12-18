---
layout: refactoring
title: Inline Function
source: Martin Fowler
source_url: https://refactoring.com/catalog/inlineFunction.html
code_smells: lazy_element
learning_hours: keyboarding
---

# 内联函数 / 内联方法（Extract function / Extract method）

## 识别
识别一个函数或方法，你想在它使用的一些或所有地方用它的主体来替换它。

## 准备
如果你打算删除原来的函数或方法，你应该列出所有使用该函数或方法的地方，这样你就可以一个一个地去内联它们。如果你只想内联一些用法，那么你可能不需要这样做。

* IDE：将光标放在函数声明上，查找使用情况。
* 可选 - "依靠编译器" - 重命名它，看看有什么问题。

## 重构
* IDE：将光标放在函数声明上，重构菜单，Inline

如果这不起作用，可以采取一些手动步骤。
* 对于每个你想内联的用法。
  * 注释出调用，这样你就可以在那里引用它了。
  * 复制函数主体，并将其粘贴到你注释出来的地方下面的调用者代码中。
  * 修复它，直到它可以编译。
  * 测试。

## 清理
* 删除任何注释过的代码
  * 如果不再使用原函数定义，则删除它。

## 后续行动
如果你在很多地方内联了一些东西，你可能已经造成了重复。你可能想为它的一部分或全部提取一个新方法。

