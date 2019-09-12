
# 题目描述

青春猪头少年，梓川咲太，又遇到麻烦了。

在咲太解决学姐的青春期症候群后没过多久，突然一名低年级女生古贺朋绘闯入了他的生活。

为了帮助朋绘摆脱纠缠她的讨厌男生，咲太勉强答应了与朋绘假扮情侣的请求。虽然他们顺利演到了暑假，并按照剧本在 $7$ 月 $18$ 日分手，第二天咲太醒来却发现整个世界被回档到了两人相遇的那一天。

在无数次回档过后，咲太从双叶理央那里得知，这样无尽的循环是“拉普拉斯妖”古贺朋绘对于未来的模拟。如果咲太想要走出循环、进入 $7$ 月 $29$ 日，他必须除去朋绘心中的某些执念。

是时候发挥咲太的嘴炮能力了！他必须在最终的表白中感化朋绘~~并以此回到和学姐没羞没臊的生活中~~。

嘴炮并不是章口就莱的。咲太已经事先预测了可能涉及的 $n$ 个话题，其中第 $i$ 个话题过后会进入 $x_i$ 个话题中的一个（若 $x_i>0$），但是**进入哪一个话题不是由咲太可以决定的**。如果一个话题没有后续的话题（即$x_i=0$），就算做表白结束。

如果从某一个话题出发，存在进入一组话题的**循环**的可能时，咲太认为这个话题不能保证成功表白。

每一个话题都有一个敏感度，敏感度越大越容易打动朋绘。咲太通过计算所有谈论到的话题的敏感度之和来评价一种表白方式的好坏，这个和越大越好。

咲太希望选择一个合适的话题作为起点，使得在保证能够成功表白的同时，让最坏情况下的敏感度之和尽可能大，并输出这个值。

# 输入格式

第一行有一个正整数 $T(1\leq T\leq 15)$，表示数据的组数。

对于每组数据，第一行有一个正整数 $n(1\le n\le 10^{5},\ \sum_{}{} n\le 5\times 10^{5})$，表示话题的总数。

第二行有 $n$ 个正整数$a_i(0\le a_i\le 10^9)$，表示话题 $i$ 的敏感度。

接下来$n$行，每行第一个数 $x_i(0\le x_i\le 10^{5},\ \sum_{}{} x_i\le 5\times 10^{5})$ 表示话题 $i$ 有可能进入的话题数量，接下来 $x_i$ 个数表示可能进入的话题编号 $id_{ij}$。

$\sum_{}{} n$ 表示输入中所有 $n$ 的和，$\sum_{}{} x_i$ 表示一组数据中所有 $x_i$ 的和。

# 输出格式

对于每组数据，输出一行。若无法保证成功表白则输出$-1$，否则输出计算的结果。

# 样例

#### 样例输入

```plain
2
6
2 3 1 1 2 5
2 2 3
2 4 5
1 6
0
0
0
4
1 2 1 2
1 2
2 1 3
1 4
0
```

#### 样例输出

```plain
6
3
```

#### 样例解释

第一组测试数据中，应选择话题 $1$ 作为起点，最坏情况下会依次进入序号为 $1,\ 2,\ 4$ 的话题，此时的敏感度之和为 $6$ 。

第二组测试数据中，应选择话题 $3$ 作为起点。若选择话题 $1,\ 2$ 作为起点则不能保证表白成功。

# 数据范围与提示


