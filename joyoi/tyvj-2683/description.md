# 

 
 # 题目描述 
<p>
Imagine that you are in a building with F floors (starting at floor 1, the lowest floor), and you have a large number of identical eggs, each in its own identical protective container. For each floor in the building, you want to know whether or not an egg dropped from that floor will break. If an egg breaks when dropped from floor i, then all eggs are guaranteed to break when dropped from any floor j ≥ i. Likewise, if an egg doesn't break when dropped from floor i, then all eggs are guaranteed to never break when dropped from any floor j ≤ i.

 
 # 输入格式 
<p>
The first line of input gives the number of cases, N. N test cases follow. Each case is a line formatted as:

 
 # 输出格式 
<p>
For each test case, output one line containing "Case #x: " followed by three space-separated integers: Fmax, Dmin, and Bmin. 
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
<tr><td>2
3 3 3
7 5 3
</td><td>Case #1: 7 2 1
Case #2: 25 3 2</td></tr></table>