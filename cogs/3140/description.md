# 题目描述


<h3>
【题目描述】
</h3>
<p>
(译者：Satoshi, 转载请注明出处)
</p>
<p>
<img src="/upload/image/20190513/20190513120500_92411.jpg" alt="" title="" width="750" height="500" align=""/> 
</p>
<p>
为了给谷仓的新畜栏省钱，奶牛贝茜开始在当地的杂戏团表演。通过在很高的平衡木上来回走动来展现她非凡的平衡感。
</p>
<p>
贝茜每次赚多少钱跟她在最终在平衡木的哪一个位置跳下来有关。平衡木从左到右的位置标为$0,1,..., N+1$。如果贝茜到达了位置$0$或者位置$N+1$她就会从平衡木的一端掉下来并且（很悲伤的）赚不到一分钱。
</p>
<p>
如果贝茜在一个给定的位置k, 她可以做下面两件事中的一件：
</p>
<p>
1. 投掷一枚硬币。如果是反面，贝茜移动到位置$k-1$；如果是正面，贝茜移动到位置$k+1$.（正反面的概率各是$\frac {1}{2}$）
</p>
<p>
2. 从平衡木上跳下来并且获得收入$f(k)$$(0&lt;=f(k)&lt;=10^9)$
</p>
<p>
因为移动取决于随机投掷硬币，贝茜意识到她不能保证任何特定的收入。然而，根据贝茜开始的位置，她想知道获得收入的最高期望(通过最合适的策略)。比如说，如果她的策略将会有$\frac {1}{2}$的机率赚到$10$块钱，$\frac {1}{4}$的机率赚到$8$块钱，$\frac {1}{2}$的机率赚到$0$块钱，那么她的收入期望将会是加权平均数$10(1/2)+8(1/4)+0(1/4)=7$。
</p>
<h3>
【输入格式】
</h3>
<p>
第一行包含一个正整数$N$。剩下的N行包含$f(1)...f(N)$
</p>
<h3>
【输出格式】
</h3>
<p>
输出$N$行，第$i$行四舍五入到收入的$10^5$倍
</p>
<h3>
【样例输入】
</h3>
<pre>2
1
3</pre>
<h3>
【样例输出】
</h3>
<pre>150000 
300000</pre>
<h3>
【提示】
</h3>
<p>
$N/A$
</p>
<p>
与标准答案差1以内即可通过
</p>
<h3>
【来源】
</h3>
<p>
http://www.usaco.org/index.php?page=viewproblem2&amp;cpid=864
</p>
<p>
USACO Dec 2018 Platinum Division
</p>
