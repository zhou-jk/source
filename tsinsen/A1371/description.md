<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　H国有n个城市，这n个城市用n-1条<b>双向道路</b>相互连通构成一棵树，1号城市是首都，也是树中的根节点。<br/>
　　H国的首都爆发了一种危害性极高的传染病。当局为了控制疫情，不让疫情扩散到边境城市（叶子节点所表示的城市），决定动用军队在一些城市建立检查点，使得从首都到边境城市的每一条路径上都至少有一个检查点，边境城市也可以建立检查点。但特别要注意的是，首都是不能建立检查点的。<br/>
　　现在，在H国的一些城市中已经驻扎有军队，且一个城市可以驻扎多个军队。一支军队可以在有道路连接的城市间移动，并在除首都以外的任意一个城市建立检查点，且只能在一个城市建立检查点。一支军队经过一条道路从一个城市移动到另一个城市所需要的时间等于道路的长度（单位：小时）。<br/>
　　请问最少需要多少个小时才能控制疫情。注意：不同的军队可以同时移动。</div>
# 输入格式

<div class="pdcont">　　第一行一个整数n，表示城市个数。<br/>
　　接下来的n-1行，每行3个整数，u、v、w，每两个整数之间用一个空格隔开，表示从城市u到城市v有一条长为w的道路。数据保证输入的是一棵树，且根节点编号为1。<br/>
　　接下来一行一个整数m，表示军队个数。<br/>
　　接下来一行m个整数，每两个整数之间用一个空格隔开，分别表示这m个军队所驻扎的城市的编号。</div>
# 输出格式

<div class="pdcont">　　共一行，包含一个整数，表示控制疫情所需要的最少时间。如果无法控制疫情则输出-1。</div>
# 样例输入

<div class="pddata">4<br/>
1 2 1<br/>
1 3 2<br/>
3 4 3<br/>
2<br/>
2 2</div>
# 样例输出

<div class="pddata">3</div>
# 输入输出样例说明

<div class="pdcont">　　第一支军队在2号点设立检查点，第二支军队从2号点移动到3号点设立检查点，所需时间为3个小时。</div>
# 数据规模和约定

<div class="pdcont">　　保证军队不会驻扎在首都。<br/>
　　对于20%的数据，2≤ n≤ 10；<br/>
　　对于40%的数据，2 ≤n≤50，0&lt;w &lt;10<sup>5</sup>；<br/>
　　对于60%的数据，2 ≤ n≤1000，0&lt;w &lt;10<sup>6</sup>；<br/>
　　对于80%的数据，2 ≤ n≤10,000；<br/>
　　对于100%的数据，2≤m≤n≤50,000，0&lt;w &lt;10<sup>9</sup>。</div>

</div>