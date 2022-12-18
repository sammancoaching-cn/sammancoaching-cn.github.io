---
layout: refactoring
title: 提炼函数（Extract Function）
source: Martin Fowler
source_url: https://refactoring.com/catalog/extractFunction.html
code_smells: long_function
learning_hours: refactoring_vocabulary
---

# 提炼函数 / 提炼方法（Extract function / Extract method）

## 识别
确定一个函数或方法的一个部分，你想把它提取到它自己的函数中。

## 准备
浏览你计划提取的那段代码，找出应该成为方法参数的变量。对它们进行 "提炼变量（Extract Variable）" 操作，并将它们移到你想提取的代码块之前。
以类似的方式，找出哪些变量被更新，并需要从新的函数中返回。如果有一个以上的变量，可以考虑提取一个以上的方法，或者创建一个新的类型，将所有的更新值封装在一个返回值中。即使你的语言支持多个返回值，考虑这一点也是明智的，因为只有一个返回值的函数更容易理解和维护。

* IDE：选择代码块并直接进行 "提取方法"。它将为你做分析并告诉你它认为你需要的参数。当你知道了你需要知道的东西后，取消重构。
* 集成开发环境："提炼变量（Extract Variable）" 可能被称为 "引入变量（Introduce Variable）"。

## 重构
* IDE：选择代码块，进行'提炼方法（Extract method）'。

如果这不起作用，这些是一些手动步骤：
* 创建一个空的新方法，用它做什么来命名，而不是用它怎么做。
* 将源方法中的代码块复制到新方法中。
* 为新方法所需的局部变量添加参数。如果这很难做到，那么你可能需要做更多的准备。回去修正一下，然后再试一次。
* 返回任何被更新的局部变量。如果不止一个，就需要做更多的准备工作--回去修正一下，再试一次。
* 编译。新的函数将是未使用的，但是应该可以编译。
* 注释掉复制的代码块，添加对新方法的调用。
* 测试。

## 清理
* 删除任何注释过的代码.
* 如果之前提取的变量不再有意义，内联方法的参数。

## 跟进
考虑新的方法是否有 [依恋情结（Feature Envy）](/code_smells/feature_envy.html)，是否应该把它移到别的地方。
