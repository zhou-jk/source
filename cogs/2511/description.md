# 题目描述


<h3>
【题目描述】
</h3>
<p>
<br/>
</p>
<p>
   学姐得到了一些萨尔那加神器碎片，对于她来说，这些超次元的神器碎片最合适的用途就是：装巧克力，然后送给学长。
</p>
<p>
   学姐拥有n种萨尔那加神器碎片，每个碎片都是一个容器，第i个碎片有ai个空槽，她可以通过俄罗斯套娃娃这样的方式把一些神器碎片组装起来，装巧克力的步骤是这样的，她首先在第一个容器的每个空槽上装上一颗巧克力，然后将第一个容器复制若干份，在第二个容器的每个空槽上装上一个第一个容器，将第二个容器复制若干份放进第三个容器……以此类推。
</p>
<p>
现在学姐想知道如果选取编号为某个连续区间的一些容器进行组装，那么最终组装出的容器能放多少颗巧克力？由于答案可能很大，你需要将它对p1取模。
</p>
<p>
   当然学姐也考虑到只吃一种巧克力的话肯定是会吃腻的，现在上有K种巧克力，她想问你在上一段的情况下，最终能组装出多少种容器？由于答案可能很大，你需要将它对p2取模。
</p>
<p>
提示：两个容器不同当且仅当它们某个空槽放的次级容器是不同的，两个一级容器（即直接用来装巧克力的容器）不同当且仅当它们某个空槽放的巧克力种类不同。注意，在容器自我复制的时候紫萱学姐可以指定它复制出的种类，也就是复制出来的容器可能与原容器不同。
</p>
<p>
<br/>
</p>
<h3>
【输入格式】
</h3>
<p>
      输入数据第一行为五个非负整数n，m，k，p1，p2，m为学姐询问的总次数，其他意义如题目所示。
</p>
<p>
      接下来一行为n个正整数，第i个数代表ai。
</p>
<p>
      接下来m行每行三个正整数ty，l，r。ty∈{1,2}，代表询问种类，询问区间为[l,r]，数据保证l≤r。
</p>
<p>
此外，若p1为0那么代表数据中不存在第一种询问，p2同理。
</p>
<p>
<br/>
</p>
<h3>
【输出格式】
</h3>
<p>
      共m行，每行一个非负整数，代表询问的答案。
</p>
<h3>
【样例输入】
</h3>
<pre>3 2 2 9 7
2 2 2
1 1 3
2 1 2
</pre>
<h3>
【样例输出】
</h3>
<pre>8
2
</pre>
<h3>
【提示】
</h3>
<p>
样例中第一个询问三个容器嵌套在一起一共有8个空位。
</p>
<p>
第二个询问第一个容器有四种（两个空位，每个空位可以放两种巧克力），第二个容器有16种，对7取模之后答案为2
</p>
<p>
<strong>【19:18更新：数据范围中k的范围】</strong> 
</p>
<p>
<img alt="" src="/upload/image/20161020/20161020191802_66157.png"/> 
</p>
<h3>
【来源】
</h3>
<p>
mzx
</p>
