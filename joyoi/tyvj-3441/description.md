# 

 
 # 题目描述 
<p>
比武大会（fight.pas\c\cpp）<br><br>【题目描述】<br>　　一年一度的天下第一比武大会又开始了，按照惯例，参赛者们围成一个圆圈，每个人可以跟他相邻的人决斗，胜利者留在原地，而失败者立刻淘汰出局。<br>　　大会的组织者已经算出每位选手的能力值，能力值大的一定可以战胜能力值小的（能力值相同时，不会有平局，必有一方被淘汰）。同时为了让比赛更激烈，他们倾向于让能力值接近的两名选手打斗。所以他们想安排一个比武的顺序，在不改变参赛者现在位置的条件下，使得所有比赛中两名选手能力值差别的总和最小。<br></p> 

 
 # 输入格式 
<p>
　　输入文件fight.in第1行1个数n，表示参赛的人数（2=<n<=200）。<br>　　第2行有n个数，依次表示圆上第1,2,…,n个人的能力值（能力值是不超过10000的非负数）。显然第n个人和第1个人相邻。<br></p> 

 
 # 输出格式 
<p>
　　输出文件fight.out包含一个整数，为n-1场比赛双方能力值差的绝对值之和的最小值。</p> 
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
<tr><td>3
2 3 1
</td><td>2</td></tr></table>
