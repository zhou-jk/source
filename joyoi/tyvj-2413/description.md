# 

 
 # 题目描述 
<p>
Irena和Sirup正准备下个周末的Party。为这个Party,他们刚刚买了一个非常大的圆桌。他们想邀请每个人，但他们现在不知道如何分配座次。Irena说当有超过K个女孩座位相邻（即这些女孩的座位是连续的，中间没有男孩）的话，她们就会说一整晚的话而不和其他人聊天。

 
 # 输入格式 
<p>
第一行有一个数T，表示以下有T组数据，每组数据有两个整数N，K。

 
 # 输出格式 
<p>
输出T行，每行顺次对应一组测试数据。
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
<tr><td>3

3 1

3 3

4 1


</td><td>2
4
3

解释：
第一组数据的方案是：MMM，MMW (M是男孩, W是女孩)。
第二组数据的方案是：MMM，MMW，MWW，WWW。
第三组数据的方案是：MMMM, MMMW,MWMW。

约束和限制：
对于20%的数据T < = 20;
对于100%的数据T < = 50;
对于20%的数据N,K < = 20;
对于100%的数据N,K < = 2000;</td></tr></table>