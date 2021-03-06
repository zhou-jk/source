
# 题目描述

**译自 [JOISC 2015](https://www.ioi-jp.org/camp/2015/2015-sp-tasks/index.html) Day1 T3「[たのしいたのしい家庭菜園](https://www.ioi-jp.org/camp/2015/2015-sp-tasks/2015-sp-d1.pdf) / [Growing Vegetables is Fun 2](https://www.ioi-jp.org/camp/2015/2015-sp-tasks/2015-sp-d1.pdf)」**

JOI 君成为了家庭菜园领域的专业人士，每年，他都在自己的菜园内种 IOI 草。如果在冬季种植 IOI 草，到春天它就会长到一定的高度。一些 IOI 草会在秋天结出美丽的果实。我们收获这些结果的 IOI 草，没有结果的 IOI 草会在冬天凋亡。

JOI 君的菜园按东西方向划为 $N$ 块田。从西向东第 $i$ 块田种植着 IOI 草 $i$。IOI 草 $i$ 在春天生长到 $H_i$ 高度，之后不生长。如果 IOI 草 $i$ 结出果实，将以 $P_i$ 元的价格卖出。没有结果的 IOI 草将不会被卖出。

春天的时候，JOI 君去了他的菜园，并决定拔去一些 IOI 草使得秋天收益最大。拔去 IOI 草 $i$ 需要 $C_i$ 元。拔去的 IOI 草将会凋亡。IOI 草只能在春天拔，不能在夏天或秋天拔。

IOI 草是一种在夏季需要大量阳光的植物。如果在菜园编号较小或较大的田里种植较高的 IOI 草，这样的话位于中间的 IOI 草就不会结果。也就是说，当 IOI 草 $i$ 未被拔走的时候，IOI 草 $i$ 在秋天能够结果当且仅当夏天时第 $1\ldots i-1$ 块田中没有比 IOI 草 $i$ 高的 IOI 草，或者第 $i+1\ldots N$ 块田中没有比 IOI 草 $i$ 高的 IOI 草。

JOI 君获得的利润是卖出 IOI 草获得的收益减去拔去 IOI 草付出的钱。JOI 君最多能获得多少利润？

给出 JOI 君的菜园的情况和田里种植 IOI 草的情况，请求出 JOI 君获得的最大利润。

# 输入格式

从标准输入读入以下内容：

第一行，一个整数 $N$，表示 JOI 的菜园有 $N$ 块田。

接下来 $N$ 行，第 $i$ 行有三个整数 $H_i,P_i,C_i$，用一个空格分隔。表示 IOI 草 $i$ 在春天长到 $H_i$ 高度，秋天如果结果能卖 $P_i$ 元，拔去这株 IOI 草要花 $C_i$ 元。

# 输出格式

输出一行一个整数到标准输出，表示 JOI 获得利润的最大值。

# 样例

#### 样例输入 1
```plain
7
22 60 30
46 40 30
36 100 50
11 140 120
38 120 20
24 90 60
53 50 20
```
#### 样例输出 1
```plain
320
```
#### 样例说明 1
考虑 IOI 草 $2$ 和 IOI 草 $7$ 被拔去的情况。剩下的 IOI 草如下表所示：

| IOI 草的编号 | IOI 草的高度 | 秋天是否会结果 |
| :----------: | :----------: | :------------: |
|     $1$      |     $22$     |       ○        |
|     $3$      |     $36$     |       ○        |
|     $4$      |     $11$     |       ×        |
|     $5$      |     $38$     |       ○        |
|     $6$      |     $24$     |       ○        |

IOI 草 $1,3,5,6$ 的卖出价格分别为 $60,100,120,90$ 元。拔去 IOI 草 $2,7$ 的花费分别为 $30,20$ 元，JOI 君的总利润为 $60+100+120+90-30-20=320$ 元，是利润最大的情况。

#### 样例输入 2
```plain
5
18 150 180
18 380 250
18 140 170
17 180 900
14 150 520
```
#### 样例输出 2
```plain
1000
```
#### 样例说明 2
在这组样例中，无需拔去任何 IOI 草，所有 IOI 草到秋天都会结果。

#### 样例输入 3
```plain
8
52 156 59
15 166 185
16 122 115
24 161 154
44 252 678
32 225 557
44 155 254
59 57 253
```
#### 样例输出 3
```plain
854
```

# 数据范围与提示

对于所有数据，$3\le N\le 10^5,1\le H_i,P_i,C_i\le 10^9$。

详细子任务附加限制及分值如下：

| 子任务编号 |                      附加条件                      | 分值 |
| :--------: | :------------------------------------------------: | :--: |
|    $1$     |                     $N\le 20$                      | $10$ |
|    $2$     |                     $N\le 300$                     | $10$ |
|    $3$     |                $N\le 5\times 10^3$                 | $10$ |
|    $4$     | 对于所有输入满足 $H_i\neq H_j\ (1\le i\lt j\le N)$ |   $50$   |
|    $5$     |                     无附加限制                     |    $20$  |



