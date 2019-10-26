
# Content

![](/source/lutece/xi-ma-la-ya-shan-shang-de-hou-zi/img/aHR0cHM6Ly9zczEuYmRzdGF0aWMuY29tLzcwY0Z2WFNoX1ExWW54R2twb1dLMUhGNmhoeS9pdC91PTI1MDYzMjQyMzIsMzkwODcyMjQwNyZmbT0yNyZncD0wLmpwZw==.jpg)

余周周告诉我喜马拉雅山上有猴子，他们知道点石成金的方法。我不信，于是余周周带我去喜马拉雅山拜访猴子。

喜马拉雅山上有n个猴子聚落，不妨叫它们1,2，…n号聚落；它们之间有m条**单向**道路(这意味着如果一条路从1号聚落到2号聚落，那么你不能通过这条路从2号聚落到1号聚落)，每条道路连接2个聚落，且拥有不同的长度。可能有两条道路的起点和终点相同，但没有一条道路的起点和终点是同一个聚落。

因为急切的想要知道点石成金的方法，余周周只想拜访四个猴子聚落，不妨按拜访顺序将它们记为A、B、C、D。当然，为了节省体力，余周周在这些城市(ABCD)之间旅行时会选择最短的路径。不过，喜马拉雅山上的风景不错，所以余周周想要多停留一会，让旅行过程当中经过的路径总长度最长。

余周周觉得自己制定旅行计划太麻烦，于是把任务交给了你。你需要帮她决定ABCD四个聚落的编号以及访问顺序，以满足余周周的要求。

# Standard Input

第一行两个整数n,m(4 ≤ n ≤ 1000, 3 ≤ m ≤ 2000), 表示喜马拉雅山上聚落的数量和单向道路的数量。

接下来m行，每行三个整数x,y,z( 1≤ x,y ≤ n, x≠y,  1 ≤ z ≤ 5000 ),表示从x到y有一条距离为z的单向道路。

输入数据保证题目有解。

# Standard Output

输出四个整数a,b,c,d，表示你选择的四个聚落的编号，按照访问顺序输出。

a,b,c,d应该各不相同。

如果有多组满足条件的答案，则输出任意一组答案。

# Samples

<style>
        table,table tr th, table tr td { border:1px solid #0094ff; }
        table { width: 200px; min-height: 25px; line-height: 25px; text-align: center; border-collapse: collapse;}   
    </style>
<table>
	<tr>
		<td>Input</td>
		<td>Output</td>
	</tr>
<tr><td>4 6
1 2 1
2 3 1
3 4 1
1 3 1
1 4 1
2 4 1</td><td>1 2 3 4</td></tr><tr><td>6 12
1 6 4
3 4 5
3 2 1
3 1 2
6 5 2
4 5 1
2 5 5
5 3 1
2 3 2
5 1 2
6 2 4
4 1 5</td><td>1 2 6 4</td></tr></table>


# Constraints



# Note

样例1：12,23,34之间的最短路距离都为1，总距离为3，显然最长。

样例2：可能有其他正确答案。

# Source

