
# 题目描述

众所周知，9011 年沃镃基苄德博士在多项式时间内解决了 $3-SAT$ 问题，从而证明了 $P=NP$。相信各位已经熟练掌握了这个技巧，接下来我们就给出一个曾经著名的 NPC 问题。

给出一张 $n$ 个点的无向图，请输出一个最大的简单环。这里简单环的定义是不经过重复顶点的环。

由于这张图比较大，我们用如下方式来生成这张图：对于 $1 \leq i<j \leq n$，$i$ 和 $j$ 两点有边当且仅当 $\gcd(i,j) \neq 1$。你需要依序输出一个最大简单环上的顶点，如果有多个最大简单环你可以输出任意一个。

# 输入格式

第一行一个正整数 $T$，表示数据组数。

接下来 $T$ 行，每行一个正整数 $n$。

# 输出格式

对于每组数据输出两行。第一行输出一个正整数 $t$，表示最大的简单环大小。

第二行输出 $t$ 个用空格分隔的正整数 $u_1,u_2 \cdots u_t$。你需要保证 $u_1,u_2 \cdots u_t$ 为互不相同的 $[1,n]$ 的整数，且 $(u_1,u_2),(u_2,u_3) \cdots (u_{t-1},u_t), (u_t,u_1)$ 间有边。

# 样例

#### 样例输入1
````
2
6
6
````
#### 样例输出1
````
3
2 6 4
3
2 4 6
````

# 数据范围与提示

对于所有数据，$1 \leq T \leq 5$，$6 \leq n \leq 500000$。

Subtask 1（10pts）：$n \leq 10$。

Subtask 2（10pts）：$n \leq 24$。

Subtask 3（20pts）：$n \leq 300$。

Subtask 4（20pts）：$n \leq 5000$。

Subtask 5（20pts）：$n \leq 50000$。

Subtask 6（10pts）：该子任务共一个测试点，$T=1$，$n=456789$。

Subtask 7（10pts）：无特殊限制。

命题人：fjzzq2002

