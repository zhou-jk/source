# 题目描述


<p>
小Y最近一直在研究某一股票，为了能够得到最大收益，他收集了这只股票近N天的走势情况。小Y手上有一笔钱，他想知道两个问题：<br/>
第一个，如果他在这N天投资一次股票，最多能获利多少钱?就是说他只买进和卖出各一次。<br/>
第二个，如果他在任意一天把资金全部买入，之后任意一天把手上的股票全部卖出，挣钱的概率是多少?挣钱是指获利大于0。当然买入当天是不允许卖的。<br/>
由于小Y这个人比较“特别”，他看中的股票也如此，没有涨停跌停的概念，爱怎么走怎么走(买这种股才够挑战)。这几天总不会一直是熊市，否则小Y干嘛在这时候投资。
</p>
<p>
输入格式<br/>
第一行，一个整数N(N≤l000)。<br/>
第二行，N个空格隔开的实数，表示每天该股票每一股的市值。
</p>
<p>
第三行，一个整数M，表示小Y手上持有的资金。
</p>
<p>
输出格式<br/>
第一行，一个实数，表示最大获利，保留3位小数。<br/>
第二行，一个实数，表示挣钱的概率，保留3位小数。
</p>
<p>
输入样例<br/>
10<br/>
5 7 6 8 5 1 2 3 4 5<br/>
100
</p>
<p>
输出样例<br/>
400.000<br/>
0.333
</p>