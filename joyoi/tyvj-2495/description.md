# 

 
 # 题目描述 
<p>
Farmer John went to cut some wood and left N (2 <= N <= 100,000)

 
 # 输入格式 
<p>
* Line 1: A single integer N

 
 # 输出格式 
<p>
* Line 1: A single integer that is the minimum number of destroyed
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
<tr><td>6
3 1
2 5
2 3
3 2
4 1
1 6
</td><td>86

OUTPUT DETAILS:

FJ returns the cows in the following order: 6, 2, 3, 4, 1, 5. While
he is transporting cow 6 to the barn, the others destroy 24 flowers;
next he will take cow 2, losing 28 more of his beautiful flora. For
the cows 3, 4, 1 he loses 16, 12, and 6 flowers respectively. When
he picks cow 5 there are no more cows damaging the flowers, so the
loss for that cow is zero. The total flowers lost this way is 24 +
28 + 16 + 12 + 6 = 86.