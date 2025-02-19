---
theme: small_steps
title: 使用TDD来写一个闰年函数
kata: leap_years
difficulty: 1
author: emilybache
---

# 使用TDD来写一个闰年函数

这通常是我和新团队做的第一个练习。你必须TDD一个接受1个整数参数并返回1个布尔值的函数。它最终是一段相当小的代码，只够展示几个TDD循环。

在我第一次演示这个Kata时，我通常不展示三角法，只做问题描述中列出的4个测试案例。这意味着我在实现第1个测试用例时直接使用模运算。这样可以缩短演示的时间，也意味着你不需要解释三角法这个概念。

## 学习目标
* 描述 "红-绿-重构 "循环
* 设计一个纯函数，使用TDD获取一个整数并返回一个布尔值

## 会议大纲

* 10分钟连接：分成两组，TDD的3个好处
* 15分钟概念：演示闰年
* 20分钟做：结对做闰年
* 10分钟思考：主要观点的总结

### 连接
两人一组。

- 想一想测试驱动开发的3个好处。

经过几分钟的讨论，请几组人向全组人说明他们想到的一些好处。把他们所说的写在白板或共享文件上。

注意--如果你认为小组对TDD的了解不够，不能提出它的任何好处，可以问一下一般的单元测试的好处。

### 演示
从白板开始，解释[LeapYear](/kata_descriptions/leap_years.html) Kata。向大家宣读描述，和/或在幻灯片上展示。在白板上写出Kata描述中给出的所有4个例子。注意，这些将变成测试。

示范如何TDD这个功能，每次举一个例子/测试。我经常使用cyber-dojo作为开发环境来做演示，因为它使TDD的周期可见。

### 做
如果你使用cyber-dojo进行练习，花几分钟时间解释如何使用它。确保他们知道如何切换打字员，如果他们是远程工作。(出去的打字员运行测试，进来的打字员刷新页面)。

让小组以两人或一群人的形式再次进行 "Kata"，从没有代码开始，只是写在白板上的例子。每隔4分钟，提醒他们换一下打字员。(或者给他们一个在线合奏的计时器）。他们应该按照你演示的方式来做，以小步骤逐一测试。

绕着两组人帮助他们。提醒他们在实现之前先写测试，逐步和迭代地工作。

如果任何一对真的很快，不需要20分钟那么长的时间，他们可以另外在另一个练习上做TDD--例如[最接近0](/kata_descriptions/closest_to_zero.html)。鼓励他们在开始编码之前做一个测试列表。

### 反思
- 想一想我们今天做了什么。如果你要向别人解释TDD的主要思想，你会怎么说？
- 用一两句话把你的解释写在便利贴或共享文件上

#### 视觉提醒
在挂图上写上 "TDD的主要思想是什么？"，用灯泡涂鸦之类的东西让它看起来有吸引力。请大家把他们的便条贴在上面。向大家宣读一些笔记。之后把海报挂在显眼的地方，也许在团队区域或咖啡室。

如果你是远程工作，那就布置这个家庭作业：请大家把他们对TDD的解释告诉另一个没有参加会议的同事，并记下他们的反应。
