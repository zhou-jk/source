# 

 
 # 题目描述 
<p>
Farmer John's N (1 <= N <= 500) cows are trying to select the

 
 # 输入格式 
<p>
* Line 1: Two space-separated integers, N and X.

 
 # 输出格式 
<p>
* Line 1: The maximum number of parent-child relationships possible on
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
<tr><td>5 8
-1 0   //第一个数字代表这头奶的产量,第二个数字代表其父亲点是哪一个.
3 1
5 1
-3 3
2 0

INPUT DETAILS:

There are 5 cows. Cow 1 can produce -1 gallons and has two daughters, cow
2 and 3, who can produce 3 and 5 gallons, respectively. Cow 3 has a
daughter (cow 4) who can produce -3 gallons. Then there's cow 5, who can
produce 2 gallons.

</td><td>2

OUTPUT DETAILS:

The best team consists of cows 1, 2, 3, and 5. Together they produce
(-1)+3+5+2 = 9 >= 8 gallons and have 2 parent-child relationships
(1--2 and 1--3). Note that a team with cows 2, 3, and 5 would be
able to produce more milk (10 gallons), but would have fewer
parent-child relationships (0).</td></tr></table>