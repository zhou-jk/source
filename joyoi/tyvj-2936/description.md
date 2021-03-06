# 

 
 # 题目描述 
<p>
农民约翰在自己的农场中发现了许多虫洞。每一个虫洞都非常特别，因为它是一条单向的道路，会把你传送到一个你进入虫洞之前的时间点！约翰的农田包含N (1 ≤ N ≤ 500)块编号为1..N的区域，M (1 ≤ M ≤ 2500)条道路以及W (1 ≤ W ≤ 200) 个虫洞。<br>由于约翰是一个时空旅行的爱好者，他希望这么做：首先从农田中某一块区域开始，沿着某些路径或者虫洞前进，并在他从起点出发以前的一个时间点回到起点。或许他会看到自己哦:) .<br>为了帮助约翰判断他的计划能否实现，他为你提供了他的F (1 ≤ F ≤ 5) 个农场的地图。走完每条路径都不会花费超过10,000的时间，每个虫洞都不会将约翰带到大于10,000 以前的时间。<br></p> 

 
 # 输入格式 
<p>
第1行：一个整数F. 接下来是F 个农场。<br>每个农场的第1行：三个用空格分开的整数N, M, and W。<br>每个农场的第2..M+1行：三个用空格分开的数字(S, E, T)，表示一条双向的连接农场S区域和E区域的路径，走完这条路径需要T 秒。两个区域可能由多条路径相连。<br>每个农场的第M+2..M+W+1行：三个用空格分开的数字 (S, E, T) ，表示一条从区域S到区域E的单向路径，该路径会使时间倒流T 秒。<br></p> 

 
 # 输出格式 
<p>
第1..F行：对于每个农场，如果约翰能够达到目标，就输出"YES"，否则输出"NO"。（输出不包括引号。）</p> 

 
 # 提示 
<p>
对于农场1，约翰无法回溯到出发前的时间。<br>对于农场2，约翰能够沿着1->2->3->1实现时间倒流，刚好回到出发时间的前1秒钟。他可以在环中的任意一点出发来实现目标。<br><br>莞中OJ上这道题的数据是比较弱的，所以如果过了本题先别得意，请将代码复制一份到POJ上提交：<br><a href="http://poj.org/problem?id=3259">3259 -- Wormholes</a><br>POJ是北京大学的Online Judgement，建议同学们也在POJ上注册一个账户，账户名和密码可以和东莞中学OJ上的一样，方便记忆。</p> 
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
3 3 1
1 2 2
1 3 4
2 3 1
3 1 3
3 2 1
1 2 3
2 3 4
3 1 8
</td><td>NO
YES</td></tr></table>
