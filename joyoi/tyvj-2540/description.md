# 

 
 # 题目描述 
<p>


 
 # 输入格式 
<p>
* Line 1 : Two space-separated integers: N and L.

 
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
4 10
1
9
11
19

INPUT DETAILS:

Four clumps: at 1, 9, 11, and 19. Bessie starts at location 10.
</td><td>
44

OUTPUT DETAILS:

Bessie can follow this route:

* start at position 10 at time 0
* move to position 9, arriving at time 1
* move to position 11, arriving at time 3
* move to position 19, arriving at time 11
* move to position 1, arriving at time 29

giving her a total staleness of 1+3+11+29 = 44.  There are other routes
with the same total staleness, but no route with a smaller one.