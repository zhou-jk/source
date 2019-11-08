# 

 
 # 题目描述 
<p>
Advanced Cargo Movement（先进货物搬运）有限公司的卡车有多种类型。有的用于运送蔬菜，有的用于搬运家具或者砖块。公司用专门的编码标识各种类型的卡车。编码很简单，只是七个小写字母组成的字符串（每个位置的字母都有特别的含义，但这对于本问题并不重要）。公司的发展史上，基于最初只有一种类型的卡车发展出多种类型的卡车，而这些卡车类型又能演变出新的卡车类型。

 
 # 输入格式 
<p>
输入包含多组数据，每组数据以一个表示卡车类型数目的整数N开头，2 <= N <= 2 000。接下来N行表示各种类型的卡车编码（一个七字母字符串）。假定所有编码都不重复。输入卡车类型数目为0时程序结束。 </p> 

 
 # 输出格式 
<p>
对于每组数据，你的程序必须输出“The highest possible quality is 1/Q”，其中 1/Q 是发展图谱的最高质量。 </p> 

 
 # 提示 
<p>
在莞中OJ提交通过后，请点击下面链接到POJ再提交一次：
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
<tr><td>4
aaaaaaa
baaaaaa
abaaaaa
aabaaaa
0
</td><td>The highest possible quality is 1/3.</td></tr></table>