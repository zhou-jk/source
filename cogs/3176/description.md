# 题目描述


<h3>
【题目描述】
</h3>
<p>
小 $D$ 有一棵树，树有 $n$ 个节点（编号 $1$ 至 $n$），边的长度均为 $1$。
</p>
<p>
小 $D$ 想知道：对于每个节点 $u$， $∑$$v$=$1$-$n$ $w[dist(u,v)]$ 是多少。
</p>
<p>
其中， $dist(u, v)$ 为 $u$, $v$ 在树上的距离， {$w_i$} 为给定序列。
</p>
<h3>
【输入格式】
</h3>
<p>
第一行，正整数 $n$。
</p>
<p>
第二行， $n$ 个自然数，第 $i$ 个元素代表$ w[i-1]$。
</p>
<p>
接下来 $n$ $-$ $1$ 行，第 $i $行两个正整数$ u_i$,$ v_i$，表示树中存在一条边连接 $u_i$ 和 $v_i$。
</p>
<h3>
【输出格式】
</h3>
<p>
输出一行， $n$ 个整数，第 $i$ 个数代表结点 $i$ 的答案。
</p>
<h3>
【样例输入】
</h3>
<pre>3
0 3 1
1 2
1 3
</pre>
<h3>
【样例输出】
</h3>
<pre>6 4 4
</pre>
<h3>
【提示】
</h3>
<p>
保证， $n$ ≤ $10^5$， $1$ ≤ $u_i$, $v_i$ ≤$ n$， $0$ ≤ $w_i $≤ $10^4$，$ w_0$ = $0$。
</p>
