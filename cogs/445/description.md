# 题目描述


<p>
【问题描述】<br/>
字符序列的子序列是指从给定字符序列中随意地(不一定连续)去掉若干个字符(可能一个也不去掉)后所形成的字符序列。令给定的字符序列x=“x0，x1，…，xn-1”， 序列Y=“y0，y1，…，yk-1是X的子序列，存在X的一个严格递增下标序 列<i0，i1，…，ik-1&gt;，使得对所有的j=0，1，…，k- 1，有xij="yj。&lt;br"> 例如，x=“ABCBDAB”，Y=“BCDB”是X的一个子序列。<br/>
对给定的两个字符序列，求出他们最长的公共子序列长度，以及最长公共子序列个数。</i0，i1，…，ik-1&gt;，使得对所有的j=0，1，…，k->
</p>
<p>
<br/>
</p>
<p>
【输入格式】
</p>
<p>
第1行为第1个字符序列，都是大写字母组成，以”.”结束。长度小于5000。<br/>
第2行为第2个字符序列，都是大写字母组成，以”.”结束，长度小于5000。
</p>
<p>
<br/>
</p>
<p>
【输出格式】
</p>
<p>
第1行输出上述两个最长公共子序列的长度。<br/>
第2行输出所有可能出现的最长公共子序列个数，答案可能很大，只要将答案对100，000，000求余即可。
</p>
<p>
<br/>
</p>
<p>
【输入样例】<br/>
ABCBDAB.<br/>
BACBBD.
</p>
<p>
<br/>
</p>
<p>
【输出样例】<br/>
4<br/>
7
</p>
