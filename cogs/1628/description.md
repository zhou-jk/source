# 题目描述


<h3>
【题目描述】
</h3>
<p>
LoadingTime几周前从他的同学那里得到了一个RNG（随机数生成器），然后他花了很长时间来学习它。他发现RNG可以在执行如下步骤后生成一个[-S,S]内的随机实数：首先RNG生成n个正整数x1……xn，这n个整数的和等于s。然后对于每个xi，它生成一个[-xi,xi]内的随机实数。RNG输出这n个生成的随机实数之和。LoadingTime注意到RNG返回值的分布很有趣，并且他希望知道，对于给定的n和x，RNG的返回值在[A,B]内的概率。你能帮助他吗？
</p>
<h3>
【输入格式】
</h3>
<p>
输入包含多组数据。
</p>
<p>
输入文件的第一行是数据组数T。
</p>
<p>
对于每组数据，第一行有三个整数n,A,B（1&lt;=N&lt;=10，-100&lt;=A&lt;=B&lt;=100）.
</p>
<p>
第二行有n个整数x1..xn（1&lt;=xi&lt;=10）.
</p>
<h3>
【输出格式】
</h3>
<p>
对每组数据，输出一行一个实数，即所求的概率。你的答案被认为正确当且仅当它和标准答案之差不超过10^-3。
</p>
<h3>
【样例输入】
</h3>
<p>
<br/>
</p>
<p>
5
</p>
<p>
1 -100 100
</p>
<p>
10
</p>
<p>
1 10 90
</p>
<p>
10
</p>
<p>
1 -20 5
</p>
<p>
10
</p>
<p>
2 -20 5
</p>
<p>
5 5
</p>
<p>
5 -5 10
</p>
<p>
1 2 3 4 5
</p>
<p>
<br/>
</p>
<h3>
【样例输出】
</h3>
<p>
<br/>
</p>
<p>
1.000000000
</p>
<p>
0.000000000
</p>
<p>
0.750000000
</p>
<p>
0.875000000
</p>
<p>
0.864720052
</p>
<p>
<br/>
</p>
<h3>
【提示】
</h3>
<p>
和SPOJ的评测方式略有不同。SPOJ上要求输出九位小数。
</p>
<h3>
【来源】
</h3>
<p>
<a href="http://www.spoj.com/problems/RNG/" target="_blank">SPOJ RNG</a>
</p>
