# 

 
 # 题目描述 
<p>
线段树的结构

 
 # 输入格式 
<p>
　　输文件为：railway.in，第一行包含三个用空格隔开的整数C、S和R，其中1≤C≤60000， l≤S≤60000，1≤R≤60000。C为城市个数，S为列车上的座位数，R为所有售票申请总数。接下来的R行每行为一个售票申请，用三个由空格隔开的整数O，D和N表示，O为起始站，D 为目的地站，N为车票站数，其中1≤D≤C，1≤O≤C，所有的售票申请按申请的时间从早到晚给出。

 
 # 输出格式 
<p>
　　输出文件为：railway.out，共有R行，每行输出一个“YES”或“NO”，表示当前的售票申请被受理或不被受理。
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
<tr><td>railway．in
4 6 4
l 4 2
l 3 2
2 4 3
l 2 3
</td><td>railway.out
YES
YES
NO
NO
