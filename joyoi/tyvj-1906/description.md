# 

 
 # 题目背景 
近来，一种新的传染病肆虐全球。蓬莱国也发现了零星感染者，为防止该病在蓬莱国<BR>大范围流行，该国政府决定不惜一切代价控制传染病的蔓延。不幸的是，由于人们尚未完<BR>全认识这种传染病，难以准确判别病毒携带者，更没有研制出疫苗以保护易感人群。于是，<BR>蓬莱国的疾病控制中心决定采取切断传播途径的方法控制疾病传播。经过&nbsp;WHO（世界卫<BR>生组织）以及全球各国科研部门的努力，这种新兴传染病的传播途径和控制方法已经研究<BR>消楚，剩下的任务就是由你协助蓬莱国疾控中心制定一个有效的控制办法。<BR> 

 
 # 题目描述 
&nbsp;研究表明，这种传染病的传播具有两种很特殊的性质；<BR>&nbsp;&nbsp;&nbsp;&nbsp;第一是它的传播途径是树型的，一个人X只可能被某个特定的人Y感染，只要Y不<BR>得病，或者是XY之间的传播途径被切断，则X就不会得病。<BR>&nbsp;&nbsp;&nbsp;&nbsp;第二是，这种疾病的传播有周期性，在一个疾病传播周期之内，传染病将只会感染一<BR>代患者，而不会再传播给下一代。<BR>&nbsp;&nbsp;&nbsp;&nbsp;这些性质大大减轻了蓬莱国疾病防控的压力，并且他们已经得到了国内部分易感人群<BR>的潜在传播途径图（一棵树）。但是，麻烦还没有结束。由于蓬莱国疾控中心人手不够，同<BR>时也缺乏强大的技术，以致他们在一个疾病传播周期内，只能设法切断一条传播途径，而<BR>没有被控制的传播途径就会引起更多的易感人群被感染（也就是与当前已经被感染的人有<BR>传播途径相连，且连接途径没有被切断的人群）。当不可能有健康人被感染时，疾病就中止<BR>传播。所以，蓬莱国疾控中心要制定出一个切断传播途径的顺序，以使尽量少的人被感染。<BR>你的程序要针对给定的树，找出合适的切断顺序。<BR> 

 
 # 输入格式 
输入格式的第一行是两个整数n（1≤n≤300）和p。表示有N个人，接下来p行，每一行有两个整数i和j，表示节点i和j间有边相连（意即，第i人和第j人之间有传播途径相连）。其中节点1是已经被感染的患者。<BR> 

 
 # 输出格式 
&nbsp;只有一行，输出总共被感染的人数。 

 
 # 提示 
noip2003提高组第4题 
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
<tr><td>7 6
1 2
1 3
2 4
2 5
3 6
3 7
</td><td>3</td></tr></table>
