
# 题目描述

> 不忘初心，继续前进。交通强国，铁路先行。

aa 在南京南火车站的站台上看着这样的标语，不由陷入了极其中二的 YY：

八万是一名憧憬着进入月域重工的月域工省的普通技术员。但是这天，八万接到了一份特殊的命令：

> <center>月域三区联合会议决议</center>
> <center>第 \*\*\* 号</center>
> <div>由援助署提出的《关于 P 国铁路隧道塌方的援助计划》已由三区联合会议审议通过，现予对外公布。</div>
> 
> <div>由于目前 Project D 处于完成前夕，军区重工及工省核心人员无法离岗，本会议决定由月域工省轨道交通部第 \*\*\* 司技术员 八万 指挥该司的 $k$ 台 \*\*\* 型挖掘机及相关作业人员前往支援。</div>
> 
> <div style="text-align:right">凤落九年腊月十五</div>

看到这份命令，八万知道自己晋升到月域重工的机会来了，他决心一定要出色的完成任务。

由于一些原因，当八万到达隧道口的时候，P 国国内尚未组织起队伍进行救援，于是八万只好指挥和他一起来的 $k$ 台挖掘机进行救援工作。

不过，八万获得了一张由 P 国提供的本次塌方隧道的线路图，图中的一些岔道口可以看作节点，岔道口之间的每段隧道可以看作是边，整个线路图可以被看作是 $n$ 个节点(分别从 $1$ 到 $n$ 标号) $m$ 条边的一个图。很快，八万利用他丰富的铁路施工经验，标出了每段隧道需要 $1$ 台挖掘机施工的时间。（由于挖掘机型号相同，质量优异，不同两台挖掘机挖掘速度相同。）

但是，八万发现，由于 P 国道路窄小，对一个轨道的疏通作业只能由一台挖掘机完成。

“怎样才能快速挖通所有隧道呢？”八万想着。

突然，他想起了他的 I 国朋友大军讲述他们国家新造的京张城际铁路背后的历史时提到的詹天佑的一些记录在他们小学课本中的一些事迹。其中，他采用了 同时施工 的办法解决了居庸关和八达岭施工慢的难题。

遗憾的是，由于他们没有带钻井设备，不能像京张铁路的八达岭隧道那样采用中部凿井法。

不过，八万成功勘探到了 $q$ 个可以开始挖掘的路口。由于编程是八万的弱项，于是他现在来求助于你来获得最短的施工时间。

正如上文所述，月域的物流水平极其发达，所以在已经挖通的道路上和不同开始挖掘的路口间转移挖掘机的速度可以忽略不计，但是为了确保安全，八万只能在岔道口指挥每个挖掘机挖一条互异的通道，并且只能在所有挖掘机挖完他当前需要的通道后才能开始进行下一次指挥。

当然，由于可能存在一些早已废弃的道路但路口原来还有人检查，导致相应的道路不需要挖通所以没有在线路图上给出但是路口给了，因而可能出现孤立的路口，忽略它们即可。

# 输入格式

本题有多组测试数据，文件第一行为测试数据组数 $T(1\leq T\leq 15)$。

对于每组测试数据，第一行为四个整数 $n,\ m,\ k,\ q(1\leq n,\ m,\ k\leq 15,\ 1\leq q\leq n)$，含义如上所示。

第二行为 $q$ 个整数，表示开始挖掘的路口所对应节点的标号。

接下来 $m$ 行每行包含三个整数 $x,\ y,\ z(1\leq x,\ y\leq n,\ 1\leq z\leq 8\times 10^6)$ 表示标号为 $x$ 的节点到标号为 $y$ 的节点有一条边，挖通这条边所对应隧道需要 $1$ 台挖掘机施工的时间。

# 输出格式

对于每一组测试数据，输出一行一个整数，表示最短的施工时间；如果不能挖通所有的通道，请输出 $-1$。

# 样例

#### 样例输入

```plain
1
8 9 3 2
1 2
1 5 2
1 3 2
2 4 2
2 6 3
3 4 4
5 6 5
5 7 3
7 8 3
8 6 2
```

#### 样例输出

```plain
10
```

# 数据范围与提示



