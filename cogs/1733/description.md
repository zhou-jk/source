# 题目描述


<h3>
【题目描述】
</h3>
<p>
Irena和Sirup正在准备他们下周末的订婚派对。他们希望邀请几乎所有人。为此他们特地买了一张巨大的圆桌。但他们现在想要知道，应该如何给人们分配座位。Irena声称，当有超过K位女士相邻时，她们就会闲聊一整晚，并且不会和其他任何人说话。
</p>
<p>
Sirup不得不同意她的看法。但，作为一名数学家，他很快开始对所有男女在圆桌旁就坐的方案数感兴趣。
</p>
<p>
将有N人坐在圆桌旁。其中的一些是男人，其余是女人。
</p>
<p>
你的任务是计算有多少种安排就坐的方式，使得没有超过K名女士相邻。
</p>
<p>
如果某种就坐方案在旋转后与另外一种方案相同，我们就认为它们是同一个方案（因此只计算一次）。
</p>
<h3>
【输入格式】
</h3>
<p>
输入数据的第一行有一个整数T，代表数据组数。
</p>
<p>
接下来是T组数据。
</p>
<p>
每组数据有一行两个整数，N（1&lt;=N&lt;=1000）和K。
</p>
<p>
对每组数据输出一个整数——安排人们就坐的方案总数，模100000007。
</p>
<h3>
【输出格式】
</h3>
<p>
在此键入。
</p>
<h3>
【样例输入】
</h3>
<p>
3
</p>
<p>
3 1
</p>
<p>
3 3
</p>
<p>
4 1
</p>
<h3>
【样例输出】
</h3>
<p>
2
</p>
<p>
4
</p>
<p>
3
</p>
<h3>
【提示】
</h3>
<p>
对于第一组数据，有两种方案：MMM或MMW（M代表男人，W代表女人）。
</p>
<p>
对于第二组数据，除上面两种之外又多了两种方案：MWW和WWW。
</p>
<p>
对于第三种数据有三种方案：MMMM，MMMW和MWMW。
</p>
<p>
至多1000组数据。
</p>
<p>
数据为随机生成。
</p>
<p>
此处的数据范围和SPOJ原题略有不同，这里N可以等于1000.
</p>
<h3>
【来源】
</h3>
<p>
<a href="http://www.spoj.com/problems/LARGE/" target="_blank">SPOJ 2734 Large Party</a> 
</p>
