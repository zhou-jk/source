# 题目描述


<h3>
【题目描述】
</h3>
<p>
输入一个n个结点的无根树的各条边，并指定一个根结点，要求把该树转化为有根树，输出各个结点的父亲编号。n≤10^6，如图所示。
</p>
<p>
<img src="/upload/image/20140524/20140524101900_74713.jpg" alt=""/> 
</p>
<h3>
【输入格式】
</h3>
<p>
<br/>
</p>
<p>
第1行：两个空格隔开的整数n，u；n是树的节点数，u是根节点编号。
</p>
<p>
第2～n行：每行包含二个整数X,Y，表示节点X，节点Y之间有边。（节点编号从0开始）
</p>
<p>
第n+1行，一个整数m
</p>
<p>
第n+2行，m个用空格隔开的整数，表示需要输出父亲的结点编号。
</p>
<p>
<br/>
</p>
<h3>
【输出格式】
</h3>
<p>
一行，m个用一个空格隔开的整数，为m个节点的父亲编号。
</p>
<h3>
【样例输入】
</h3>
<pre>8 1
0 1 
0 2 
0 3 
1 4 
1 5 
5 6 
5 7
8
0 1 2 3 4 5 6 7 </pre>
<h3>
【样例输出】
</h3>
<pre>1 -1 0 0 1 1 5 5。 
</pre>
<h3>
【提示】
</h3>
<p>
1号节点没有父亲，输出-1。
</p>
<h3>
【来源】
</h3>
<p>
《算法竞赛入门经典（第2版）》第11章例题
</p>
