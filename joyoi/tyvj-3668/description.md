# 

 
 # 题目描述 
<p>
玩具 [Chen Hu, 2006]

 
 # 输入格式 
<p>
* 第 1 行: 六个用空格隔开的整数 D, N1, N2, C1, C2, Tc

 
 # 输出格式 
<p>
 第 1 行: 提供玩具所需要的最小费用.
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
<tr><td>4 1 2 2 1 3
8
2
1
6

输入解释:
Bessie想开4天的party, 第1天需要8个玩具, 第2天需要2个玩具, 第3天需要1个玩具,
第4天需要6个玩具. 第一种方式需要$2, 用时1天; 第二种方式需要$1, 用时2天. 买
一个玩具需要$3.

</td><td>
35
输出解释:
第 1 天   买8个玩具, 花去$24; 送2个玩具去快洗, 6个慢洗.
第 2 天   取回2个快洗的玩具, 花去$4. 送1个玩具去慢洗.
第 3 天   取回6个慢洗的玩具, 花去$6.
第 4 天   取回所有的玩具(与现有的加在一起正好6个), 花去$1. 这样就用了最少的钱.
</td></tr></table>