
# 题目描述

在 $1\sim n$ 的所有全排列中，逆序对数量为 $k$ 的有多少个。由于答案可能很大请将答案对 $10^9+7$ 取模。

注：在一个全排列 $p_i$ 中，若点对$(i,j)$ 满足 $i<j$ 且 $p_i>p_j$ 则称 $(i,j)$ 为一对逆序对。

# 输入格式

第一行一个整数 $T(1\leq T \leq 10^6)$ ,代表数据组数。

下面 $T$ 行每行两个整数 $n,\ k(1\leq n,\ k\leq 5000)$ 分别为排列的长度和逆序对的数量。


# 输出格式

$T$行，每行一个整数，代表答案对 $10^9+7$ 取模的值。

# 样例

#### 输入样例

```plain
3
4 6
10 10
233 666
```

#### 输出样例

```plain
1
21670
386608145
```


# 数据范围与提示


