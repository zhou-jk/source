<div id="pcont1" style="margin-top:20px; display:block;">
<div class="pdcont">　　﻿</div>
# 问题描述

<div class="pdcont">　　比特兰正在尝试在Bit-X行星上进行一项太空任务。由于Bit-X的反动领袖Bitonix规律性的在这个行星的轨道上巡逻，他们的任务将十分复杂。<br/>
　　围绕着Bit-x有n个太空站，按顺时针方向从1到n编号。这些太空站均匀的分布在一个环形轨道上，所以编号为i和i+1（1≤i＜n），以及编号为1和n的太空站相邻。每一对相邻的太空站之间的距离都是相等的m太空米。每次巡逻，Bitonix的火箭将在一个太空站发射，然后在沿着轨道航行任意一段距离（不可以为零）后，在任意一个（包括出发的那个）太空站结束这一次巡逻。<br/>
　　Bitonix的火箭以燃料为动力。在Bitonix装上一个x升的燃料箱并且选择了方向（顺时针或是逆时针）之后，这个火箭将沿着选定的方向顺着这个圆形轨道恰好飞行x太空米。注意这个火箭没有制动装置，因此在用光这个燃料箱之前这个火箭不可能停下来。<br/>
　　例如，假设n=3，m=60，Bitonix有容量为10，60，90，100升的燃料箱。如果Bitonix从太空站1开始巡逻，用100升的燃料箱顺时航行，然后用90升的燃料箱顺时针航行，最后用10升的燃料箱逆时针航行，他将回到太空站1。这构成了一次有效的巡逻。注意Bitonix不需要将所有的燃料箱都用上。在这个例子中，对Bitonix来说另一种有效地巡逻方式是简单地用60升燃料箱飞到太空站2或是3。<br/>
　　然而，如果n=3，m=60，并且对Bitonix来说可以使用的燃料箱只有一个10升的和一个100升的，他将无论如何也无法进行一次有效地巡逻（他不能完成任何一个恰好停在太空站的巡逻）。<br/>
　　比特兰空间机构想要摧毁Bitonix的燃料箱中的一部分，从而使Bitonix无法完成任何有效地巡逻。找出多少种这个机构可以阻止Bitonix完成巡逻的破坏组合，并输出这个答案对1000000007（10^9+7）取模。</div>
# 输入格式

<div class="pdcont">　　输入的第一行包括三个整数n（2≤n≤1000）——太空站的数目，m（1≤m≤120）——相邻太空站之间的距离，和t（1≤t≤10000）——Bitonix所拥有的燃料箱的数目。<br/>
　　输入第二行包括t个用空格分开的在1到10^9（包括1和10^9）之间的整数，表示Bitonix的燃料箱的体积。</div>
# 输出格式

<div class="pdcont">　　输出一个单独的整数——比特兰空间机构为了阻止Bitonix完成巡逻所可以破坏的不同子集的数目，对10^9+7取模。</div>
# 样例输入

<div class="pddata">7 6 5<br/>
5 4 12 6 5</div>
# 样例输出

<div class="pddata">6</div>
# 样例输入

<div class="pddata">3 60 2<br/>
10 100</div>
# 样例输出

<div class="pddata">4</div>
# 数据规模和约定

<div class="pdcont">　　对于10%的数据，t≤10；<br/>
　　对于30%的数据，m≤70；<br/>
　　对于60%的数据，m≤100；<br/>
　　对于100%的数据，2≤n≤1000，1≤m≤120，1≤t≤10000，每个燃料箱的容量不超过10^9。<br/>
　　<b>注意</b>：所有的燃料箱都是不同的，即使它们有相同的容量。<br/>
　　<b>P.S.</b>：其实众大神们不用关注这个m的范围的……主要是本弱菜第一次出数据，实在搞不懂那个有梯度、有区分度是怎么搞的，所以最后就把我做题过程中经历过的几个程序拿出来跑了一下。鉴于我的做法时间比较受m的影响，所以就按照这几个程序被卡的范围把m的梯度弄出来了，o(╯□╰)o。但是本傻叉的程序显然无法跟大神们的相提并论，所以这个m的范围也肯定代表不了什么。所以众大神们真的真的不用考虑这个m的范围有什么含义……</div>

</div>