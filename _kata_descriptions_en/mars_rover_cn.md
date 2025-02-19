---
title: Mars Rover - 火星漫游者
kata_name: mars_rover
---

# 火星漫游者

美国国家航空航天局（NASA）的一队机器人漫游车将在火星的一个高原上着陆。

这个高原是奇怪的长方形，必须由漫游车来导航，以便它们的车载相机能够获得周围地形的完整视图，并传送到地球。

漫游车的位置由一个X和Y坐标以及一个代表指南针四点之一的字母组合来表示。高原被划分为一个网格，以简化导航。一个例子是0，0，N，这意味着漫游器在左下角，面向北方。

为了控制漫游车，NASA发送了一串简单的字母。可能的字母是 "L"、 "R" 和 "M"。
"L" 和 "R"使漫游车分别向左或向右旋转90度，而不离开其当前位置。

"M"意味着向前移动一个网格点，并保持相同的方向。

假设从(x, y)向北的正方形是(x, y+1)。

## 输入

第一行输入的是高原的右上角坐标，左下角坐标被假定为0,0。

其余的输入是与已经部署的漫游器有关的信息。每个漫游器有两行输入。第一行是漫游器的位置，第二行是一系列的指令，告诉漫游器如何探索高原。

位置由两个整数和一个用空格隔开的字母组成，对应于x和y坐标以及漫游器的方向。

每个漫游器将按顺序完成，这意味着在第一个漫游器完成移动之前，第二个漫游器将不会开始移动。

## 输出

每个漫游器的输出应该是它的最终坐标和方向。

测试输入。

5 5

1 2 N

LMLMLMLMM

3 3 E

MMRMMRMRRM

预期的输出。

1 3 N

5 1 E

### 鸣谢
此Kata在[Google code](https://code.google.com/archive/p/marsrovertechchallenge/)上有描述。
