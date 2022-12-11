---
layout: code_smell
title: 过长的消息链（Message Chains）
source: Martin Fowler
---

# 过长的消息链（Message Chains）
当客户端向一个对象请求另一个对象，然后请求另一个对象，以及另一个对象的链。在 Java 这样的语言中，它可能看起来像`A.getB().getC().getD().getE()'。如果链中的一个对象的结构有任何变化，它可能是相当脆弱的--变化会传播，并可能产生比你想的更广泛的影响。这种坏味道是你打破 [迪米特法则](https://en.wikipedia.org/wiki/Law_of_Demeter) 时产生的。
