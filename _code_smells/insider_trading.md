---
layout: code_smell
title: 内幕交易（Insider Trading）
source: Martin Fowler
---

# 内幕交易（Insider Trading）
类或模块对彼此的内部细节了解太多。它们之间可能会传递 private 数据。这说明它们之间的耦合太紧密了。这种情况经常发生在子类和它的父类之间 —— 子类可以接触到太多本应属于父类的细节。