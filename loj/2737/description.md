
# 题目描述

**题目译自 [JOISC 2016](https://www.ioi-jp.org/camp/2016/2016-sp-tasks/index.html) Day3 T3 「[電報](https://www.ioi-jp.org/camp/2016/2016-sp-tasks/2016-sp-d3.pdf)」**    

给出 $N$ 个点，每个点的出度**均为 $1$**，给出这 $N$ 个点初始指向的点 $A_i$，和改变这个点指向的目标所需要的价值 $C_i$。  
求让所有点强连通的最小花费。


# 输入格式

第一行输入一个数 $N$ 表示点的个数。  
之后的 $N$ 行每行两个数 $A_i$ $C_i$ 表示第 $i$ 个点指向第 $A_i$ 个点，更改该点指向的点花费为 $C_i$。 

# 输出格式

共一行，为让所有点强连通的最小花费。

# 样例

#### 样例输入 1
```plain
4
2 2
1 4
1 3
3 1
```

#### 样例输出 1
```plain
4
```

#### 样例解释 1

<!-- img src="https://i.loli.net/2018/12/10/5c0dfb9730859.png" width="30%" / -->

![telegram.png](/source/loj/2737/img/aHR0cHM6Ly9sb2otaW1nLnVweXVuLm1lbmNpLm1lbXNldDAuY24vMjAyMC8wNy8wMi81ZWZkNGU2MDUzNjhhLnBuZw==.png)

很显然，把 $2 \rightarrow 1$ 的这条边改成 $2 \rightarrow 4$（花费 4）的情况下构成强连通分量花费最小。

#### 样例输入 2
```plain
4
2 2
1 6
1 3
3 1
```

#### 样例输出 2
```plain
5
```

#### 样例解释 2
很显然把 $1 \rightarrow 2$ 的这条边改成 $1 \rightarrow 4$ 花费 2，把 $3 \rightarrow 1$ 的这条边改成 $3 \rightarrow 2$ 花费 3 的情况下构成强连通分量花费最小，总花费为 5。  

#### 样例输入 3
```plain
4
2 2
1 3
4 2
3 3
```

#### 样例输出 3
```plain
4
```

#### 样例输入 4
```plain
3
2 1
3 1
1 1
```

#### 样例输出 4
```plain
0
```

# 数据范围与提示

对于全部的数据，$1 \leq N \leq 10^{5}$ ,$1 \leq A_i \leq N$ ,   $A_i \neq i$  , $1 \leq C_i \leq 10^{9} $。

具体子任务限制及得分情况如下表：

| Subtask |      限制      | 分数 |
| :-----: | :------------: | :--: |
|   $1$   | $1 \leq N \leq 10 $ | $10$ |
|   $2$   | $1 \leq N \leq 15$ | $30$ |
|   $3$   | $1 \leq N \leq 3000$ | $30$ |
|   $4$   | 无追加限制 | $30$ |

