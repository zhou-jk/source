# 

 
 # 题目描述 
<p>
　　求一个图的最小生成树。这个图边较少，但点较多（n <= 5000），宜用kruskal算法。

 
 # 输入格式 
<p>
　　第一行一个数n，表示无向图的顶点的数量，接下来从第2行到第n+1行，每行有n个数（0表示相应点之间无边直接相连，不为0表示相应点之间有边直接相连，其值即为相连边的权值），形成一个n*n的矩阵，用以表示这个无向图。

 
 # 输出格式 
<p>
　　一行，仅一个数，表示最小生成树的边权值和。</p> 

 
 # 提示 
<p>
基于贪心的kuruskal算法求最小生成树，算法思路如下：
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
<tr><td>8
0 9 4 6 0 0 0 0
9 0 0 2 0 0 0 0
4 0 0 1 9 0 0 0
6 2 1 0 0 2 6 0
0 0 9 0 0 3 0 0
0 0 0 2 3 0 0 7
0 0 0 6 0 0 0 2
0 0 0 0 0 7 2 0
</td><td>自己算。</td></tr></table>