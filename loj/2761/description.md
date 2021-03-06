
# 题目描述

**译自 [JOI 2013 Final](https://www.ioi-jp.org/joi/2012/2013-ho/index.html) T1「[電飾](https://www.ioi-jp.org/joi/2012/2013-ho/2013-ho.pdf)」**

每年 JOI 高中的文化祭上，走廊上都会有彩灯装饰。共有 $ N $ 个彩灯，从走廊的西侧到东侧排成一列。每个彩灯要么亮要么不亮。

JOI 高中的仓库里沉睡着一台能够对彩灯进行操作的机器。对于指定的连续的一段彩灯，此机器能将这些彩灯中所有亮的变成不亮的，所有不亮的变成亮的。但是由于这个机器已经老化了，所以最多只能使用一次。

JOI 高中的学生们很喜欢彩灯的交替列（亮的彩灯和不亮的彩灯交替排列的一段连续的彩灯）。他们希望能够在必要时使用一次这个机器，使得所有彩灯中所含的最长的交替列最长。

#### 例子
例如，彩灯从西向东依次为：

![TIM20180807230724.png](/source/loj/2761/img/aHR0cHM6Ly93d3cuejRhLm5ldC9pbWFnZXMvMjAxOC8wOC8wNy9USU0yMDE4MDgwNzIzMDcyNC5wbmc=.png)

（$ ○ $ 表示亮的彩灯， $ ● $ 表示不亮的彩灯）。此时，对从第 $ 4 $ 个彩灯到第 $ 7 $ 个彩灯进行操作。

![TIM20180807230736.png](/source/loj/2761/img/aHR0cHM6Ly93d3cuejRhLm5ldC9pbWFnZXMvMjAxOC8wOC8wNy9USU0yMDE4MDgwNzIzMDczNi5wbmc=.png)

这样，第 $ 2 $ 个彩灯到第 $ 8 $ 个彩灯之间的彩灯组成了长为 $ 7 $ 的交替列。

![TIM20180807230748.png](/source/loj/2761/img/aHR0cHM6Ly93d3cuejRhLm5ldC9pbWFnZXMvMjAxOC8wOC8wNy9USU0yMDE4MDgwNzIzMDc0OC5wbmc=.png)

另外，可以对第 $ 8 $ 个彩灯进行操作。

![TIM20180807230754.png](/source/loj/2761/img/aHR0cHM6Ly93d3cuejRhLm5ldC9pbWFnZXMvMjAxOC8wOC8wNy9USU0yMDE4MDgwNzIzMDc1NC5wbmc=.png)

这样，第 $ 4 $ 个彩灯到第 $ 10 $ 个彩灯之间的彩灯组成了长为 $ 7 $ 的交替列。

![TIM20180807230804.png](/source/loj/2761/img/aHR0cHM6Ly93d3cuejRhLm5ldC9pbWFnZXMvMjAxOC8wOC8wNy9USU0yMDE4MDgwNzIzMDgwNC5wbmc=.png)

使用一次此机器不可能有长度为 $ 8 $ 或以上的交替列。

#### 任务
给出每个彩灯的情况，求出在最多使用一次机器的情况下，最长交替列长度的最大值。

# 输入格式

输入标准如下：
- 第一行为一个整数 $ N $；  
- 第二行为 $ N $ 个以空格分开的数字 $ 0 $ 或 $ 1  $ ，表示机器操作前的彩灯的情况。第 $ i(1 \leq i \leq N) $ 个数字表示从西侧开始的第 $ i $ 个彩灯的状态，为 $ 1 $ 表示彩灯是亮的，为 $ 0 $ 表示彩灯是不亮的。

# 输出格式

输出一行一个整数：表示可能的最长交替列的最大长度。

# 样例

#### 输入样例 1
```plain
10
1 1 0 0 1 0 1 1 1 0
```
#### 输出样例 1
```plain
7
```
#### 样例说明 1
这就是题目描述中的例子。
#### 输入样例 2
```plain
10
1 0 0 0 0 1 0 1 0 1
```
#### 输出样例 2
```plain
8
```
#### 样例说明 2
对从西侧开始的第 $ 4 $ 个彩灯进行操作，得到长度为 $ 8 $ 的最长交替列。
#### 输入样例 3
```plain
5
1 1 0 1 1
```
#### 输出样例 3
```plain
5
```
#### 样例说明 3
对从西侧开始第 $ 2 $ 个彩灯到第 $ 4 $ 个彩灯进行操作，所有彩灯共同构成最长交替列。
#### 输入样例 4
```plain
3
0 1 0
```
#### 输出样例 4
```plain
3
```
#### 样例说明 4
注意：存在不使用机器而能达到最大值的情况。

# 数据范围与提示

对于 $ 20\% $ 的分值：
- $ N \leq 500 $

对于 $ 40\% $ 的分值：
- $ N \leq 2000 $

对于 $ 100\% $ 的数据：
- $ 2 \leq N \leq 10^5 $

