# 

 
 # 题目描述 
<p>


 
 # 输入格式 
<p>
* Line 1: Two space-separate integers, N and K

 
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
<tr><td>
13 4
0
1
0
2
4
6
8
6
8
8
9
11
12</td><td>
5

OUTPUT DETAILS:

FR builds five supports (at locations 1, 5, 7, 9, and 13). The steel
is tangent to the ground at four locations: 1-5, 5-7, 7-9, and
12-13.

If FR only builds supports at the four locations 1, 5, 9, and 13,
then the steel would be below ground from 5-9. If FR built supports
at 1, 7, and 13, then -- although the steel is always above ground
-- supports 7 and 13 are more than 4 units apart horizontally. There
is no solution using fewer than 5 supports such that no two consecutive
supports are more than 4 units apart horizontally.</td></tr></table>