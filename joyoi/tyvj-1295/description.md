# 

 
 # 题目背景 
"牵起你的手，我觉得很温柔。"经过一番艰苦的努力，小v终于和他的MM订婚了，在婚礼这天，由于小v的朋友实在太多，而酒店座位不够，所有小v只好设置一些考验来谢绝一些朋友的到来。<BR> 

 
 # 题目描述 
小v的朋友们被关在一个很旧的房间里，房间里有n*m块地板，每个地板都有一个承载值Vi，而小v的朋友们站在这房间里的地板上（没有人在同一块地板），现在他们要走出这个房间。<BR>&nbsp;&nbsp;&nbsp;规定两个相邻的地板间距离为1，而每个人只能上下或左右移动到距离不超过d的地板上，每次某个人离开了某个地板，那么该地板的承载值就会减1，当其等于零时，别的人就不可踏上这块地板。<BR>&nbsp;&nbsp;&nbsp;只有彻底离开房间边界以外才算成功逃离，在逃离的过程中，任何时刻都不能有两个人在同一个地板上，你的任务是求最多能逃离的人数。<BR><BR> 

 
 # 输入格式 
第一行为一个整数p，表示有p组<BR>	然后有若干组数据，每组数据分别为：<BR>		第一行为两个整数n，d，n表示房间里地板的行数，d如题意所示。<BR>	然后为两个矩阵，第一个矩阵Sij表示房间里地板的情况，第二矩阵表示房间里人的分布情况，P代表有人，.代表无人。<BR><BR> 

 
 # 输出格式 
P行每行一个整数，分别表示每组最大的逃离数<BR> 

 
 # 提示 
数据范围：<BR>	对于50%的测试点，0&lt;n&lt;=15,0&lt;=d，Sij&lt;=5,p&lt;=10<BR>	对于100%的测试点，0&lt;n&lt;=25,0&lt;=d，Sij&lt;=9,p&lt;=25<BR><BR> 
# 样例数据
<style>
        table,table tr th, table tr td { border:1px solid #0094ff; }
        table { width: 200px; min-height: 25px; line-height: 25px; text-align: center; border-collapse: collapse;}   
    </style>
<table>
	<tr>
		<td>输入样例</td>
		<td>输出样例</td>
	</tr>
<tr><td>4
3 1
1111
1111
1111
PPPP
PPPP
PPPP
3 2
00000
01110
00000
.....
.PPP.
.....
3 1
00000
01110
00000
.....
.PPP.
.....
5 2
00000000
02000000
00321100
02000000
00000000
........
........
..PPPP..
........
........

</td><td>10
3
0
3

</td></tr></table>
