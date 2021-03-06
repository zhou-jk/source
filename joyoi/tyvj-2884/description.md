# 

 
 # 题目描述 
<p>
dd_engi所在的TIANYI公司要举办一次盛大的公司聚会。可惜的是，由于场地和花费的原因，不可能所有人都参加。现在的任务是拟定参加聚会人员的名单。<br>TIANYI公司的组织架构可以看做一棵有根多叉树。也就是说，在编号为1~N的所有N名员工中，除了最高管理者（编号为1）以外，每个员工都有且仅有一位直接上司；最高管理者则是这棵多叉树的“根”。这很好理解，对吗？另外，我们保证，员工的编号会大于他的直接上司的编号。<br>不同的员工对于聚会有着不同的要求，事实上，若邀请第i位员工（编号为i），在聚会中满足他的要求需要花费Ci元。另一方面，不同的员工在聚会中的“兴奋指数”也不同，第i位员工参加聚会的兴奋指数是Ei。<br>选择参加聚会的人员还有一个限制：为了使参加聚会的员工能够尽量放松，若邀请了某位员工，就不能邀请他的任何一位上司。这里“上司”的定义是这样的：最高管理者没有上司，其余所有员工的直接上司以及直接上司的所有上司都是他的上司。换句话说，某位员工的上司就是树中从他的节点走到根节点的路径上经过的所有节点（包括根结点，但不包括他自身）。<br>在满足上述限制的前提下，dd_engi希望参加聚会人员的兴奋指数之和最大，但同时他被告知，满足所有参加聚会人员的要求的总花费不得超过M元。那么，参加聚会人员的名单究竟应该怎样确定才最优呢？你需要求出的是最大的总兴奋指数。<br></p> 

 
 # 输入格式 
<p>
第一行，两个空格隔开的整数，N与M。<br>第二行，N-1个整数，分别是第2位至第N位员工的直接上司的编号。<br>第三行，N个整数，分别是C1、C2……CN。<br>第四行，N个整数，分别是E1、E2……EN。<br></p> 

 
 # 输出格式 
<p>
只需输出一行一个整数，即最大的总兴奋指数。</p> 

 
 # 提示 
<p>
数据范围<br>30%的数据满足N<=20。<br>100%的数据满足1 <= N <= 1024, 0 <= M <= 109, 0 <= Ci <= 1024, -1024 <= Ei <= 1024。<br></p> 
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
<tr><td>10 100
1 2 2 1 4 3 5 6 1
12 53 127 32 164 22 199 10 19 17
-1 0 3 5 7 -2 9 6 8 13
</td><td>27</td></tr></table>
