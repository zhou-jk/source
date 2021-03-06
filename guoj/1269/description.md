
# 题目描述

一辆自动驾驶的士正在 Innopolis 的街道上行驶。该街道上有 $n+1$ 个停车站点，它们将街道划分成了 $n$ 条路段。每一路段都拥有一个路灯。当第 $i$ 个路灯亮起，它将照亮连接第 $i$ 与第 $i+1$ 个站点的路段。否则这条路段将是黑暗的。

出于安全性的考虑，自动驾驶的士只能行驶在被照亮的路段上。换言之，的士能从站点 $a$ 出发到达站点 $b(a<b)$ 的条件是：连接站点 $a$ 与 $a+1$,$a+1$ 与 $a+2$，$\ldots$，$b−1$ 与 $b$ 的路段都被照亮。

在经过一些意外故障或修理之后，街道上的路灯可能是亮起的，也可能是熄灭的。

现在给定 $0$ 时刻时，街道上路灯的初始状态。之后 $1,2,\ldots, q$ 时刻，每时刻会发生下列两种事件之一：

- “`toggle` $i$” — 切换第 $i$ 个路灯的状态。具体地说，若路灯原来亮起，则现在将熄灭；若路灯原来熄灭，则现在将亮起。
- “`query` $a\ b$” — 自动驾驶的士部门的负责人想知道，从 $0$ 时刻起到当前时刻，有多少个时刻满足：自动驾驶的士能够从站点 a 出发到达站点 b。

请你帮助自动驾驶的士部门的负责人回答他们的问题。

# 输入格式

第一行包含两个整数 $n$ 和 $q(1\le n,q\le 300 000)$ —— 表示路灯的数量与时刻数。

第二行包含一个字符串 $s$ 表示路灯的初始状态 $(|s|=n)$，$s_i$ 为 ‘`1`’ 表示第 $i$ 个路灯初始时亮起；$s_i$ 为 ‘`0`’ 表示第 $i$ 个路灯初始时熄灭。

接下来 $q$ 行每行描述一个时刻的事件。第 $i$ 行描述时刻 $i$ 所发生的事件。

- “`toggle` $i$”$(1\le i\le n)$ —— 该时刻切换了第 $i$ 个路灯的状态。
- “`query` $a\ b$”$(1\le a<b\le n+1)$ —— 计算从 $0$ 时刻起到该时刻，共有多少个时刻满足的士能从站点 $a$ 出发到达站点 $b$。

至少有一个时刻的事件是 `query`。

# 输出格式

对于每个 `query` 的事件，输出一行单个整数，表示该问题的答案。

# 样例

#### 样例输入
```plain
5 7
11011
query 1 2
query 1 2
query 1 6
query 3 4
toggle 3
query 3 4
query 1 6
```

#### 样例输出
```plain
1
2
0
0
1
2
```
#### 样例解释
在样例中

|时刻|路灯状态|询问|答案对应的时刻|
|:-:|:-:|:-:|:-:|
|$1$|`11011`|||
|||`query 1 2`|$1$|
|$2$|`11011`|||
|||`query 1 2`|$1,2$|
|$3$|`11011`|||
|||`query 1 6`|无|
|$4$|`11011`|||
|||`query 3 4`|无|
|$5$|`11011`|||
|||`toggle 3`||
|$6$|`11111`|||
|||`query 3 4`|$6$|
|$7$|`11111`|||
|||`query 1 6`|$6,7$|

# 数据范围与提示

在**测试数据**中，子任务 1 是样例数据，因此相应的 Subtask 编号 +1。

#### Subtask 1 (points: 20)
$n\le 100, q\le 100$。

#### Subtask 2 (points: 20)
对于所有 “`query `$a\ b$” 事件，满足 $b−a=1$。

#### Subtask 3 (points: 20)
对于所有 “`toggle `$i$” 事件，第 $i$ 个路灯将被点亮。

#### Subtask 4 (points: 20)
所有 `toggle` 事件都发生在第一个 `query` 事件之前。

#### Subtask 5 (points: 20)
无特殊限制。

