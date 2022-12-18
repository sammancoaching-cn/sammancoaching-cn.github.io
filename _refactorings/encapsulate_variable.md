---
layout: refactoring
title: 封装变量（Encapsulate Variable）
source: Martin Fowler
source_url: https://refactoring.com/catalog/encapsulateVariable.html
code_smells: global_data
learning_hours: primitive_obsession
---

# 封装变量/封装字段（Encapsulate Variable / Encapsulate Field）

## 识别
确定一个变量或字段，它具有公共或全局访问权限，你想将其封装起来。

## 准备
找到它的所有使用位置，并存储这个列表或重新创建它的方法。

* IDE：将光标放在函数声明上，查找使用情况。
* 或者--"依靠编译器"--重命名它，看看有什么问题。

## 重构
* 为你要封装的字段创建一个 getter 和 setter 函数。
  * IDE：将光标放在字段上， "重构，封装"（在顶部菜单） 或 "生成... Getter 和 Setter"。
* 编译/运行静态检查。
* 浏览每个变量或字段的引用，用对 getter 或 setter 函数的调用来代替它。使用你之前做的列表。
* 在每次替换后进行测试。

在这一点上，你已经成功地达到了最初的目的--全局变量被 getter 和 setter 函数封装起来了。

## 清理

将封装的字段或变量改为私有（如果你的语言允许）。

## 跟进

* 如果你有几个相关的字段，你可以提取 Class。给它起个好名字。
* 现在它被封装了，你可以更容易地改变字段的类型。例如 [以对象取代基本类型（Replace Primitive with Object）](replace_primitive_with_object.html)。

