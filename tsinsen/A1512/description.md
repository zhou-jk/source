<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<pre class="pddata"><span lang="zh-CN">上帝永远将一切几何化。——柏拉图<br/><br/>功成名就的金先生开始研究起哲学来了。他做了一个梦，梦见他拥有了一个理想国！<br/>他的理想国山明水秀，风光旖旎。城市繁荣，交通发达。土地平旷，屋舍俨然，有桑竹美池良田之属，阡陌交通，鸡犬相闻。<br/>把理想国的城市标号为1至n，每个城市有一个独立的编号。在地图上，可以建立一个平面直角坐标系，用一个坐标表示一座城市的位置。一些城市间修建了笔直的高速公路。公路一共有m条。为了避免相撞事故，除端点外，任两条公路没有公共点。理想国的城市是双连通的，亦即任何两个城市间可以找到两条不相交的简单路径。<br/>金先生的理想国的每个城市的繁荣程度不同，最繁荣的繁荣度为1,最破败的繁荣度为n。一条公路两端的城市的繁荣度如果分别为a和b(a &lt; b)，那么称开区间(a, b)为这条公路的特征区间。观察两条公路，它们的路况相似，当且仅当它们的特征区间的交非空。<br/>金先生一觉醒来，只记得理想国城市布局，而忘了城市的繁荣情况了。于是，他想解决下面两个问题。<br/>(1) 平均情况下，相似的路有几对？<br/>(2) 最好情况下，最多能有几条路，它们两两相似？</span>
</pre>

# 输入格式

<pre class="pddata"><span lang="zh-CN">第一行两个整数n, m，代表城市数和公路数。<br/>接下来n行，每行两个整数，代表标号为i的城市在地图上的坐标。<br/>接下来m行，每行两个整数，为一条公路连接的两个城市的编号。</span>
</pre>

# 输出格式

<pre class="pddata"><span lang="zh-CN">仅一行，用空格分开，表示两小问的答案。第一问的答案保留小数点后</span>3<span lang="zh-CN">位。</span>
</pre>

# 样例输入

<div class="pddata">3 3<br/>
1 9<br/>
2 8<br/>
0 0<br/>
1 2<br/>
2 3<br/>
3 1</div>
# 样例输出

<pre class="pddata">2.000 2
</pre>

# 数据规模和约定

<pre class="pddata"><span lang="zh-CN">对10%的数据，n &lt;= 9。<br/>对20%的数据，n &lt;= 13。<br/>另有30%的数据，布局分别为简单多边形，网格图，三角形带。<br/>另有10%的数据，包含不超过10行，每行全是正方形或三角形，每个正方形行的正方形个数不超过10，每个三角形行的三角形个数不超过20。<br/>另有10%的数据，包含不超过13个面。<br/>对于100%的数据，n &lt;= 100，坐标绝对值在30000以内。我们约定，三角形带为形如下图所示的形状。其中，它的一组平行边平行于坐标轴。不仅如此，网格图的边也平行于坐标轴。</span>
</pre>
<div class="pdcont"><img width="864" height="540" src="source/tsinsen/A1512/img/aHR0cDovL3d3dy50c2luc2VuLmNvbS9SZXF1aXJlRmlsZS5kbz9maWQ9QjVRSGpoamc=.do"/></div>

</div>