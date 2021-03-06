
# 题目描述

小皮与妹子们欢乐的玩耍着，直到小 S 的看到了这一幕，世界终于清静了下来……

小 S 非常的生气，于是决定报复社会，于是出了这么一道题来为难小皮：

给出$n$个字符串$S$，你需要支持以下操作：

- 1 在字符串$x$后面插入一个字符$y$
- 2 询问字符串$x$在第$y$次操作后，在当前的字符串$z$中出现的次数
- 3 询问$n$个串中，本质不同的子串的个数
- 4 输入一个字符串$T$，判断$T$在$n$个字符串中出现次数最多的一个中出现的次数

小皮发现自己根本无处下手，只好把他的终身幸福寄托在了你的身上。

# 输入格式

第一行输入一个整数$n$和参数$t$。$t=1$时表示强制在线，$t=0$时不强制在线。

接下来$n$行，每行一个输入字符串。

接下来一行输入一个整数$m$，表示操作次数。

接下来$m$行，每行首先输入$op$，表示操作类型。

- `1 x y` 表示在第$x$个字符串后面插入一个字符$y$，其中$y$需要解密得到，$y = (y \operatorname{xor} lastans) \bmod 10$
- `2 x y z` 表示询问字符串$x$在第$y$次操作后，在当前的字符串$z$中出现的次数
- `3` 询问本质不同子串的个数
- `4 T` 其中$T$是一个字符串，判断$T$在$n$个字符串中出现次数最多的一个中的出现次数

其中$lastans$为上一次$2, 4$操作得到的答案，$3$操作无需考虑。

# 输出格式

对于每一个操作$2, 3, 4$，输出一行表示答案。

# 样例

**样例 1 输入**
```
3 0
121
123
1
4
1 3 2
3
2 3 0 1
4 12
```

**样例 1 输出**
```
8
2
1
```

**样例解释**

对于第一次询问：本质不同的字符串有`1, 2, 12, 21, 121, 3, 23, 123`，共$8$种。

对于第二次询问：`1`在`121`中出现了$2$次。

对于第三次询问：`12`在三个串中都出现了$1$次，所以最大出现次数为$1$。

本题有附加样例，请自行下载。

# 数据范围与提示

- 对于$20\%$的数据：$n \leq 10, Q \leq 100, \sum |S| \leq 200, \sum |T| \leq 1000$；
- 对于另外$20\%$的数据：不包含$2$操作；
- 对于另外$30\%$的数据：$T=0$；
- 对于$100\%$的数据：$n \leq 20, Q \leq 2 \times 10^5, \sum |S| \leq 2 \times 10^5, \sum |T| \leq 2 \times 10^7$

出题人：Hankpipi NaVi_Awson

来源：HNOI 2018 省队集训 Day 6 T3

