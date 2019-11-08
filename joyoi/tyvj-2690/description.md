# 

 
 # 题目描述 
<p>
一个港口被分成了 M个区域(1<=M<=10)，每个区域最多允许同时停靠10000 艘船，只要这些船来去的时间不互相冲突.每艘船都只能停靠在特定的一个区域。有n 艘船(1<=N<=100000)，已知每条船的到达时刻、离开时刻和它应该进入的区域。求一个调度方案使得能有最多的船得以停靠。</p> 

 
 # 输入格式 
<p>
Input contains many test sets. A test data set is defined as follow:

 
 # 输出格式 
<p>
For each test data set you should output one integer, the maximal number of the berthed ships, per line.

 
 # 提示 
<p>
2004年广东省大学生程序竞赛试题 Problem B</p> 
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
<tr><td>2 6  //二个区域,六只船
3   //区域的大小
3  //区域的大小
1 2 1  //每只船来去的时间及它应该要停泊的区域号
1 2 1
1 2 1
1 2 1
1 2 2
1 2 2

1 3
2
1 3 1
2 6 1
2 8 1

1 4
2
1 3 1
5 6 1
2 8 1
4 10 1
</td><td>5
2
3