
# Description

<div class="content"><p><span style="font-size: medium">1.wqs喜欢模拟飞行。<br/>
　　2.clj开了一家神犇航空，由于clj还要玩游戏，所以公司的事务由你来打理。<br/>
　　注意：题目中只是用了这样一个背景，并不与真实/模拟飞行相符<br/>
</span></p>
<div class="pdsec"><span style="font-size: medium">问题描述</span></div>
<div class="pdcont"><span style="font-size: medium">　　神犇航空有一架航班从A地飞往B地，需要规划一条最经济的飞行线路。为了简化问题，我们认为地面是一个平面，高度为0，上有N个航路点，有M条双向航线，每条航线连接两个航路点，有两个参数H和W，表示以h高度通过这条航路，费用为(H-h)<sup>2</sup>+W。在每个航路点可以爬升/下降高度，每爬升一个高度需要费用C，而下降不需要费用。航路点0为A地，N-1为B地。<br/>
</span></div>
<p></p></div>

# Input

<div class="content"><div class="pdcont"><span style="font-size: medium">　　第一行3个正整数，N,M和C，含义如题目所述；<br/>
　　以下M行，每行4个整数，u,v,H,W，表示u,v之间有一条航线，H,W为描述中的两个参数。<br/>
</span></div></div>

# Output

<div class="content"><div class="pdcont"><span style="font-size: medium">　　仅一行，一个整数，表示A地到B地的最小费用。<br/>
</span></div></div>

# Sample Input

<div class="content"><span class="sampledata">3 2 5<br/>
0 1 10 10<br/>
1 2 20 10<br/>
<br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata">114<br/>
<br/>
</span></div>

# Hint

<div class="content"><p></p><p>数据规模和约定<br/><br/>
　　对于10%的数据，N,M&lt;=5，H&lt;=200；<br/><br/>
　　另有20%的数据，N&lt;=100，M&lt;=500，H&lt;=100；<br/><br/>
　　对于全部的测试数据，N&lt;=2000，M&lt;=10000，C&lt;=10，0&lt;=u,v&lt;N，0&lt;=H&lt;=10^5，0&lt;=W&lt;=2*10^5；输入保证答案不超出32位有符号整型。<br/><br/>
</p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

