# 

 
 # 题目描述 
<p>


 
 # 输入格式 
<p>
* Line 1: A single integer: N

 
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
7
B
B
F
B
F
B
B

INPUT DETAILS:

There are seven cows and they are facing backward, backward, forward,
backward, forward, backward, and backward, respectively.
</td><td>
3 3

OUTPUT DETAILS:

For K = 3, the machine must be operated three times: turn cows (1,2,3),
(3,4,5), and finally (5,6,7):

      B > F   F   F
      B > F   F   F
      F > B > F   F
      B   B > F   F
      F   F > B > F
      B   B   B > F
      B   B   B > F