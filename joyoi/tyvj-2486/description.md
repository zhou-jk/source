# 

 
 # 题目描述 
<p>
N (1 <= N <= 50,000) cows conveniently numbered 1..N are driving

 
 # 输入格式 
<p>
* Line 1: Four space-separated integers: N, M, D, and L

 
 # 输出格式 
<p>
* Line 1: A single integer representing the maximum number of cows
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
<tr><td>3 1 1 5//三头牛开车过一个通道.当一个牛进入通道时，它的速度V会变成V-D*X(X代表在它前面有多少牛),它减速后，速度不能小于L
5
7
5

INPUT DETAILS:

There are three cows with one lane to drive on, a speed decrease
of 1, and a minimum speed limit of 5.

</td><td>2

OUTPUT DETAILS:

Two cows are possible, by putting either cow with speed 5 first and the cow
with speed 7 second.
