# 

 
 # 题目描述 
<p>
N(1 ≤ N ≤ 1000)个农场中的每个农场都有一只奶牛去参加位于第X个农场的聚会.共有M (1 ≤ M ≤ 100,000)条单向的道路,每条道路连接一对农场.通过道路i会花费Ti (1 ≤ Ti ≤ 100)的时间. 

 
 # 输入格式 
<p>
第1行:三个用空格隔开的整数. 

 
 # 输出格式 
<p>
唯一一行:一个整数: 所有参加聚会的奶牛中,需要花费总时间的最大值. 
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
<tr><td>4 8 2
1 2 4
1 3 2
1 4 7
2 1 1
2 3 5
3 1 2
3 4 4
4 2 3
</td><td>
10
样例说明: 

共有4只奶牛参加聚会,有8条路,聚会位于第2个农场. 

第4只奶牛可以直接到聚会所在地(花费3时间),然后返程路线经过第1和第3个农场(花费7时间),总共10时间. 