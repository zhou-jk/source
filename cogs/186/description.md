# 题目描述


<p>
n个被自然地编号为1..n奶牛（1&lt;=n&lt;=1000）正在同样被方便的编号为1..n的n个牧场中吃草。更加自然而方便的是，第i个奶牛就在第i个牧场中吃草。
</p>
<p>
其中的一些对牧场被总共的n-1条双向通道的一条连接。奶牛可以通过通道。第i条通道连接的两个牧场是A_i和B_i（1&lt;=A_i&lt;=N;1&lt;=B_i&lt;=N）其长度是L_i（1&lt;=L_i&lt;=10000）。
</p>
<p>
通道只会连接两个不同的牧场，所以这些通道使得整个牧场构成了一棵树。
</p>
<p>
奶牛们是好交际的希望能够经常的访问别的奶牛。急切地，它们希望你能通过告诉它们Q（1&lt;=Q&lt;=1000）对牧场的路径来帮助他们安排旅行。（这里将有Q个询问，p1,p2(1&lt;=p1&lt;=n；1&lt;=p1&lt;=n)）
</p>
<p>
分数：200
</p>
<p>
问题名称：pwalk
</p>
<p>
输入格式：
</p>
<ul>
<li>
第1行：两个用空格隔开的整数：n和Q
</li>
<li>
第2..n行：第i+1行包含三个用空格隔开的整数：A_i,B_i和L_i
</li>
<li>
第n+1..N+Q行：每行包含两个用空格隔开的整数，代表两个不同的牧场，p1和p2
</li>
</ul>
<p>
输入样例（file pwalk.in）：
</p>
<pre>4 2
2 1 2
4 3 2
1 4 3
1 2
3 2
</pre>
<p>
输出格式：
</p>
<ul>
<li>
第1..Q行：行i包含第i个询问的答案。
</li>
</ul>
<p>
输出样例：
</p>
<pre>2
7
</pre>
<p>
输出说明：
</p>
<p>
询问1：牧场1和牧场2的路径长度为2。 询问2：3-&gt;4-&gt;1-&gt;2;总长为7。
</p>
