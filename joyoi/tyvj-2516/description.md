# 

 
 # 题目描述 
<p>
Farmer John's N (1 <= N <= 50,000) cows are standing in a very

 
 # 输入格式 
<p>
* Line 1: A single integer, N.

 
 # 输出格式 
<p>
* Line 1: The loudest moo volume heard by any single cow.
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
4 2
3 5
6 10

INPUT DETAILS:

Three cows: the first one has height 4 and moos with volume 2, etc.
</td><td>7

OUTPUT DETAILS:

The third cow hears both the first and second cows moo 2+5=7.  Though the
third cow moos with volume 10, no one hears her.