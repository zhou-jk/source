# 

 
 # 题目描述 
<p>
在程序设计中，正则表达式(Regular Expressions)是用来处理复杂的字符串匹配以及模式识别问题的利器。正则表达式的一种常见用法是，给定一个正则表达式和一个字符串，然后询问给定的正则表达式能否匹配整个字符串，你需要处理的就是这种询问。

 
 # 输入格式 
<p>
第一行是一个简化版的正则表达式。

 
 # 输出格式 
<p>
对于第二行开始的每个字符串，根据能否进行匹配，输出一行“Regular Expression is Fun!”或者“Boring String Matching...”，不包括引号，其中的标点是英文标点（半角）。</p> 

 
 # 提示 
<p>
数据范围
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
<tr><td>[Dd]{2}_[eE][n-n][g_v][ii-jj]
dd_engi
Dd_engi
DD_envj
dD_eegi
dd-engi
ddengi
DD_Enhi
</td><td>Regular Expression is Fun!
Regular Expression is Fun!
Regular Expression is Fun!
Boring String Matching...
Boring String Matching...
Boring String Matching...
Boring String Matching...