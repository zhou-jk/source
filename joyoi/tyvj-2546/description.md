# 

 
 # 题目描述 
<p>
Bessy 正在上学并且分数还不错. 她考了N (一个数据中1 <= N <= 50,000, 其

 
 # 输入格式 
<p>
*第一行: N

 
 # 输出格式 
<p>

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
<tr><td>5
1 2
5 9
3 8
4 10
1 3

输入解释:

Bessy 考了5门试, 分数分别为1/2, 5/9, 3/8, 4/10, 1/3.
</td><td>2
1
2

输出解释:

当D=1时, 去掉1/3将使总分变成13/29, 而去掉3/8则得到11/24.

当D=2时, 去掉1/3和3/8得到总分10/21. 更高的7/14则能由去掉3/8和4/10
得到.