# 题目描述


<h3>
【题目描述】
</h3>
<p>
<br/>
</p>
<p>
    FJ建的新牛棚里有N（2&lt;=N&lt;=3,000,000）个栏位，这N个栏位围成了一个巨大的环形，N个栏位编号依次为0～N-1，其中0号栏位与N-1号栏位相邻。
</p>
<p>
    到了晚上，FJ的牛会陆续返回牛棚。在每头牛心里都有一个他们最钟意的栏位，然而，如果某头牛最钟意的栏位已经被别的牛抢先占领了，他会从该栏位开始按顺序依次查看后面的栏位，直到找到第一个未被占领的栏位为止，他将占领这个栏位。如果他查看到了N-1号栏位仍未找到空位，他将从0号栏位开始继续找下去。
</p>
<p>
    给定每头牛所钟意的栏位号，请计算：当所有牛都回栏后，未被占领的牛栏中编号最小的那个。请注意本题的答案跟牛返回牛棚的顺序无关。
</p>
<p>
    为避免大量读入数据的问题，输入数据只有K（1&lt;=K&lt;=10,000）行，每行的格式为：X Y A B
</p>
<p>
    其中指定了X*Y头牛最钟意的栏位，即每X头牛依次钟意的栏位为f(1)～f(Y)，其中f(i)=(A*i+B) mod N；A,B均在0到1,000,000,000之间。
</p>
<p>
         切记标准内存限制为64MB。
</p>
<p>
<br/>
</p>
<h3>
【输入格式】
</h3>
<p>
<br/>
</p>
<p>
第1行：两个空格隔开的整数N，K；
</p>
<p>
 第2～K+1行：每行包含四个整数X,Y,A,B，含义如上所述。牛的总数不超过N-1，可能有若干行数据都涉及到相同的栏位。
</p>
<p>
<br/>
</p>
<h3>
【输出格式】
</h3>
<p>
一行，即求未被占领的栏位中编号最小者。
</p>
<h3>
【样例输入】
</h3>
<pre>10 3
3 2 2 4
2 1 0 1
1 1 1 7
<p>
输入解释：共有10个栏位，编号为0～9；第2行数据显示有3头牛钟意6（(2*1+4)mod 10=6）号栏位,另外3头牛钟意8（(2*2+4)mod 10=8）号栏位；第3行数据显示有2头牛钟意1（(0*1+1)mod 10=1）号栏位；第4行数据显示有1头牛钟意8（(1*1+7)mod 10=8）号栏位（共有4头牛钟意这个栏位）。
</p>
</pre>
<h3>
【样例输出】
</h3>
<pre><p>
5
</p>

<p>
输出解释：

除了5号栏位，其它栏位均被占领。          
</p>
</pre>
<h3>
【提示】
</h3>
<p>
在此键入。
</p>
<h3>
【来源】
</h3>
<p>
USACO 2013 November Contest, Gold
</p>
