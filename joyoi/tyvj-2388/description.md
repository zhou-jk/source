# 

 
 # 题目描述 
<p>
<img border="0" src="/source/joyoi/tyvj-2388/img/aHR0cDovL3d3dy5qb3lvaS5jbi9wcm9ibGVtL3R5dmotMjM4OC9wcm9ibGVtc19pbWFnZXMvMjc4Mi8xNTA3XzEuanBn.jpg">

 
 # 输入格式 
<p>
输入文件editor.in的第一行是指令条数t，以下是需要执行的t个操作。其中：

 
 # 输出格式 
<p>
输出文件editor.out的每行依次对应输入文件中每条GET指令的输出。
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
<tr><td>15
Insert 26
abcdefghijklmnop
qrstuv wxy
Move 16
Delete 11
Move 5
Insert 1
^
Next
Insert 1
_
Next
Next
Insert 4
.\/.
Get 4
Prev
Insert 1
^
Move 0
Get 22
</td><td>.\/.
abcde^_^f.\/.ghijklmno