# 

 
 # 题目背景 
<p>NOIP2014提高组第二题</p> 

 
 # 题目描述 
<p>无向连通图G有n个点，n-1条边。点从1到n依次编号，编号为i的点的权值为Wi&nbsp;&nbsp;，每条边的长度均为1。图上两点(u,&nbsp;v)的距离定义为u点到v点的最短距离。对于图G上的点对(u,&nbsp;v)，若它们的距离为2，则它们之间会产生<strong>W</strong><strong>u</strong><strong>&times;</strong><strong>W</strong><strong>v</strong>的联合权值。</p>

<p>请问图G上所有可产生联合权值的<strong>有序点对</strong>中，联合权值最大的是多少？所有联合权值之和是多少？</p> 

 
 # 输入格式 
<p>输入文件名为link.in。</p>

<p>第一行包含1个整数n。</p>

<p>接下来n-1行，每行包含2个用空格隔开的正整数u、v，表示编号为u和编号为v的点之间有边相连。</p>

<p>最后1行，包含n个正整数，每两个正整数之间用一个空格隔开，其中第i个整数表示图G上编号为i的点的权值为Wi。</p>

<p>输入样例：</p>

<p>5</p>

<p>1&nbsp;2</p>

<p>2&nbsp;3</p>

<p>3&nbsp;4</p>

<p>4&nbsp;5</p>

<p>1&nbsp;5&nbsp;2&nbsp;3&nbsp;10</p> 

 
 # 输出格式 
<p>输出文件名为link.out。</p>

<p>输出共1行，包含2个整数，之间用一个空格隔开，依次为图G上联合权值的最大值和所有联合权值之和。<strong>由于所有联合权值之和可能很大，输出它时要对10007取余。</strong></p>

<p><strong>输出样例：</strong></p>

<p>20&nbsp;74</p> 

 
 # 提示 
<p>对于30%的数据，1&lt;n&le;100；</p>

<p>对于60%的数据，1&lt;n&le;2000；</p>

<p>对于100%的数据，1&lt;n&le;200,000，0&lt;Wi&nbsp;&le;10,000。</p> 
