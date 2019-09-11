
# 题目描述

蒟蒻$\text{kanekik}$因为水水水被教练捉了，教练没有像往常一样惩罚$\text{kanekik}$长跑十千米，深蹲$100$下，仰卧起坐$100$下....而是让他去处理校门口那颗歪脖子树......歪脖子树有许多节点，每个节点上都有一个权值，每处理一个节点都需要花费体力。\
伐木是一件枯燥且乏味的累活，因为$\text{kanekik}$编程很弱，并且机房大佬Melantha不愿帮助$\text{kanekik}$（因为$\text{kanekik}$太菜了），请你来帮助$\text{kanekik}$，让他尽量轻松一些。\
\
\
这颗树有$n$个节点，$n-1$条边，无环，每个节点上有一个权值w。

你可以进行合并操作，选择一条边的两个端点$a$、$b$，合并$a$、$b$，消耗的体力值以及合并后点的权值为$a$,$b$节点权值的较大值。

$\text{kanekik}$很懒很怕累，希望你帮助他伐木，设计一个最优的方案，使整棵树大小为一（只有一个节点）时，消耗的体力总值最小。

# 输入格式

输入共 2n 行

第一行，一个整数n,表示共有n个节点

接下来n行，第i+1行一个整数w，表示第i个节点的权值为w

接下来$n-1$行，每行两个整数$u$,$v$，表示$u$,$v$之间有一条边相连

# 输出格式

输出共一行，一个整数，表示体力消耗总和的最小值
（答案取模$998244353$)

# 样例

输入#1:
```
3
1
2
3
1 2
2 3
```
输出#1:
```
5
```

# 数据范围与提示

数据范围

对于$100%$的数据 $n\leq 2000000$

数据点$1$  $n=3$

数据点$2$  $n=10$

数据点$3\ 4\ 5\ 6\ $数据随机

数据点$7\ 8$ $n\leq 1000000$

数据点$9\ 10$ $n\leq 2000000 $
