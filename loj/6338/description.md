
# 题目描述

#### 原题来自：[Codeforces Round #182 (Div 1). E. Yaroslav and Arrangements](https://codeforces.com/problemset/problem/301/E)

如果一个数列相邻两项之差的绝对值均为 $1$（我们认为首项和末项也相邻），并且首项是数列中最小的元素之一，那么我们称之为良好数列。

如果一个数列单调不降且长度在 $1$ 到 $n$ 之间，数列中每个数的值在 $1$ 到 $m$ 之间，且重排后能得到至少 $1$ 个至多 $k$ 个良好数列（意思是说将这个数列打乱顺序可以使数列变成良好数列，而且能得到的不同的良好数列的数量在 $1$ 到 $k$ 之间，两个数列不同当且仅当存在某一位置上的数不同），那么我们称之为优秀数列。

给出 $n$、$m$、$k$，求优秀数列的个数。

答案对 $10^9 + 7$ 取模 。

# 输入格式

单独一行三个整数 $n , m , k$，以单个空格间隔。

# 输出格式

单独一行输出答案。

# 样例

#### 样例输入 1
```plain
1 1 1
```

#### 样例输出 1
```plain
0
```
#### 样例解释 1

长为 $1$ 的数列都不是良好数列，因为首项与末项是相邻的，且是相同的，不满足绝对值相差 $1$ 的条件。

长为 $1$ 的数列重排后还是长为 $1$ 的数列，一定不能得到良好数列，所以没有优秀数列。

#### 样例输入 2
```plain
3 3 3
```

#### 样例输出 2
```plain
2
```

#### 样例解释 2

一个优秀数列是 ${1, 2}$，它重排能得到 ${1,2}$ 和 ${2,1}$，其中只有 ${1,2}$ 是良好数列，所以重排能够得到 $1$ 个良好数列，满足条件。

另一个优秀数列是 ${2,3}$ 。

#### 样例输入 3
```plain
28 15 34
```

#### 样例输出 3
```plain
54737
```
#### 样例 3 举例

如 ${2,2,3,3,3,4}$ 能重排得到 $2$ 个良好数列，分别是 ${2,3,4,3,2,3}$ 和 ${2,3,2,3,4,3}$。$2$ 在 $1$ 到 $34$ 之间，所以这是一个优秀数列。

但如果输入改成 $28\ 15\ 1$，那么由于 $2$ 超过了 $k$，所以 ${2,2,3,3,3,4}$ 将不再是优秀数列。

# 数据范围与提示

对于 $30\%$ 的数据，$n,m,k \leq 8$；

对于 $60\%$ 的数据，$n,m,k \leq 30$；

对于 $100\%$ 的数据，$n,m,k \leq 100$。


