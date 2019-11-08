# 

 
 # 题目描述 
<p>
Farmer John is on a boat seeking fabled treasure on one of the N

 
 # 输入格式 
<p>
* Line 1: Two space-separated integers: N and M

 
 # 输出格式 
<p>
* Line 1: The minimum danger that Farmer John can encounter while
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
<tr><td>3 4
1
2
1
3
0 5 1
5 0 2
1 2 0

INPUT DETAILS:

There are 3 islands and the treasure map requires Farmer John to
visit a sequence of 4 islands in order: island 1, island 2, island
1 again, and finally island 3. The danger ratings of the paths are
given: the paths (1, 2); (2, 3); (3, 1) and the reverse paths have
danger ratings of 5, 2, and 1, respectively.


</td><td>7

OUTPUT DETAILS:

He can get the treasure with a total danger of 7 by traveling in
the sequence of islands 1, 3, 2, 3, 1, and 3. The cow map's requirement
(1, 2, 1, and 3) is satisfied by this route. We avoid the path
between islands 1 and 2 because it has a large danger rating.