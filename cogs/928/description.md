# 题目描述


<!--
题目名称： 一起进军全国吧
文件名称： zengokuhe
题目难度： 5
时间限制： 1 s
空间限制： 128 MiB
测试点数： 10
评测方法： 过滤换行回车
-->
<blockquote>21 世紀、世界の麻雀競技人口は一億人の大台を突破。<br/>
日本でも大規模な全国大会が毎年開催され、プロに直結する成績を残すべく高校麻雀部員達が覇を競っていた。<br/>
これはその頂点を目指す少女達の軌跡……。
</blockquote>
<h3>
题目背景
</h3>
<p>
21世纪，世界上的麻将竞技人口超过了数亿，专业的麻将选手受到人们的关注，在高中也每年都举办大规模的全国麻将大赛，在那里，为了留下能够进军职业选手的战绩，高中麻将部员们相互争霸，这就是向着顶点进军的少女们的轨迹！
</p>
<p>
不管是阿知贺的鸭子对小和和的追求，还是清澄岭上使与原村的约定，她们都要一起进军全国，留下一段百合佳话。
</p>
<h3>
题目要求
</h3>
<p>
全国比赛一定是在一个地方举行，不会像联赛一样还能分省区举办。本题设定全国赛在首都举行。
</p>
<p>
我们给出铁路线路数据，要求求出给定站点到全国赛区的最短路程。
</p>
<h3>
输入格式
</h3>
<ul>
<li>
输入文件第一行为一个整数 n 和一个字符串 s ，表示以下有 n 次询问站点 a_i 到首都 s 的最短距离。
</li>
<li>
下面 n 行，每行一个字符串表示站点名称。
</li>
<li>
接下来是铁路线路图。每条线路都以<code>S 线路名</code>作为第一行，下面直到下一条线路或文件结束，每行描述一个在该线路上的站点：
<ol>
<li>
可能是<code>站点 路程</code>，
</li>
<li>
可能是<code>路程 站点</code>；
</li>
<li>
行首没有多余字符，但一行之后还可能有一些其他数据（比如几等座、票价、实际运行路程等），这都应该忽略掉。
</li>
</ol>
站点为一个不含空格的字符串。（实际站点可能有东西南北之分，但为了简化问题，输入数据已将其视为一个站点的自环，你应该知道怎么做。）里程数为实数，表示从线路起点到该站的路程。
</li>
</ul>
<h3>
样例输入
</h3>
<pre>3 東京
長野
上海
大阪
S 東海道新幹線
東京 0.0 0.0
名古屋 366.0 342.0
京都 513.6 476.3
大阪 552.6 515.4
S 東北新幹線
0.0 東京
3.6 上野
30.3 大宮
S 上越新幹線
大宮 0.0
高崎 74.7
S 北陸新幹線
高崎 0.0 0.0
長野 117.4 117.4</pre>
<h3>
输出格式
</h3>
<ul>
<li>
输出有 n 行，第 i 行表示站点 a_i 与首都的距离，评测插件判断该答案与标准答案差距不超过 0.1 即可算做正确。如果暂时没有这样的通路，请输出 -1 。每答对一个询问得到 1/n 的分数。
</li>
</ul>
<h3>
样例输出
</h3>
<pre>222.40
-1.00
552.60</pre>
<h3>
数据范围及要求
</h3>
<ul>
<li>
只有两组测试数据，第一组是日本新干线主要线路，第二组是中国八横八纵铁路线路。都使用 ANSI 编码。
</li>
<li>
询问量 n 不大于站点数。
</li>
</ul>
<h3>
数据来源
</h3>
<p>
数据从维基百科上手工复制粘贴，稍加批处理形成一定格式，可能在处理中出现一些失误导致结果不符合实际情况，不必理会。
</p>
