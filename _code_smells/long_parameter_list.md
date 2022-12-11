---
layout: code_smell
title: 过长参数列表（Long Parameter List）
source: Martin Fowler
---

# 过长参数列表（Long Parameter List）
如果参数列表很长，那么你的函数或方法可能很难理解和推理。有时一组参数会形成一个 [数据泥团（Data Clumps）](data_clumps.html)，这给了你一个如何解决的线索。(把它们都移到一个类上，然后直接传入这个类）。通过引入 [全局数据（Global Data）](global_data.html)来减少参数列表的大小，通常不是一个好主意。