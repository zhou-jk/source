
# 题目描述

小 y 是一个喜爱游戏的女孩子。

这天，小 w 和小 y 在玩一个经营国家的游戏。这个国家有一些交通线路，且这些线路呈一棵树的形状。

这个国家一共有$n-1$个城市和$n$个乡村，其中城市从$1$到$n−1$编号，乡村从$1$到$n$编号，且$1$号城市是首都。道路都是单向的，本题中我们只考虑从乡村通往首都的道路网络。

对于每一个城市，恰有一条公路和一条铁路通向这座城市。对于城市$i$，通向该城市的道路（公路或铁路）的起点，要么是一个乡村，要么是一个编号比$i$大的城市。没有道路通向任何乡村。除了首都以外，从任何城市或乡村出发只有一条道路；首都没有往外的道路。从任何乡村出发，沿着唯一往外的道路走，总可以到达首都。
小 y 在游戏中获得了一笔资金，她决定用这笔资金来改善交通。由于资金有限，她只能翻修任意的$n-1$条道路。

她希望从乡村通向城市可以尽可能地便利，于是根据人口调查的数据，她对每个乡村制定了三个参数，编号为$i$的乡村的三个参数是$a_i$，$b_i$和$c_i$。假设从编号为$i$的乡村走到首都一共需要经过$x$条未翻修的公路与$y$条未翻修的铁路，那么该乡村的不便利值为$c_i*(a_i+x)*(b_i+y)$。

在给定的翻修方案下，每个乡村的不便利值相加的和为该翻修方案的不便利值。翻修$n-1$条道路有很多方案，其中不便利值最小的方案称为最优翻修方案，小 y 自然希望找到最优翻修方案。请你帮助她求出这个最优翻修方案的不便利值。

# 输入格式

第一行为正整数$n$。

接下来$n−1$行，每行描述一个城市。其中第𝑖行包含两个数$s_i, t_i$。$s_i$表示通向第$i$座城市的公路的起点，$t_i$表示通向第$i$座城市的铁路的起点。如果$s_i > 0$，那么存在一条从第$s_i$座城市通往第$i$座城市的公路，否则存在一条从第$-s_i$个乡村通往第$i$座城市的公路；$t_i$类似地，如果$t_i > 0$，那么存在一条从第$t_i$座城市通往第$i$座城市的铁路，否则存在一条从第$−t_i$个乡村通往第$i$座城市的铁路。

接下来$n$行，每行描述一个乡村。其中第𝑖行包含三个数$a_i, b_i, c_i$，其意义如题面所示。

# 输出格式

输出一行一个整数，表示最优翻修方案的不便利值。

# 样例

**样例 1 输入**
```
6
2 3
4 5
-1 -2
-3 -4
-5 -6
1 2 3
1 3 2
2 1 3
2 3 1
3 1 2
3 2 1
```

**样例 1 输出**
```
48
```

本题有附加样例，请自行下载。

# 数据范围与提示

Subtask #1 (10'): $n \leq 12$。

Subtask #2 (20'): $n \leq 50$。

Subtask #3 (30'): $n \leq 2000$。

Subtask #4 (40'): $n \leq 20000$。

对于$100\%$的数据，$1 \leq a_i, b_i \leq 60, 1 \leq c_i \leq 10^9$，任意乡村可以通过不超过$40$条道路到首都。

本题将使用捆绑测试。

出题人：wfj

来源：HNOI 2018 省队集训 Day 4 T1


