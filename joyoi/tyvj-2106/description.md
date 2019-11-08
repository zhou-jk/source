# 

 
 # 题目背景 
<p>农夫约翰想要给他的奶牛照相。他的N头奶牛排列在一条笔直的道路上，第i头牛的坐标为xi，并且要么是纯白牛，要么是斑点牛。没有两头奶牛占据同一个位置。</p> 

 
 # 题目描述 
<p>约翰想要给一段连续的奶牛照相。为了公平，他想要确保斑点牛和纯白牛的数量在相片中一样多。为了使相片更美观，约翰带上了一桶油漆，这样他就可以把任意数量的纯白牛&ldquo;粉刷&rdquo;成斑点牛。请你帮约翰计算他在确保公平的前提下，能拍摄到相片的最大尺寸（即最右边奶牛的坐标与最左边奶牛的坐标之差）。</p>

<p>（当然，约翰也可以选择不粉刷任何牛，如果必要的话。）</p> 

 
 # 输入格式 
<p>第一行一个整数N&nbsp;。接下来N行包含了N头牛的信息：一个整数xi以及一个字符W（代表纯白牛）或S（代表斑点牛）。</p> 

 
 # 输出格式 
<p>一行，约翰可能拍摄到相片的最大尺寸。</p> 

 
 # 提示 
<p>样例解释：约翰可以拍摄位置从3到10的相片，其中有3头纯白牛，1头斑点牛。约翰只需要把其中一头纯白牛粉刷成斑点牛即可。</p>

<p>数据范围：</p>

<p>对于30%的数据，2&lt;=N&lt;=1000</p>

<p>对于100%的数据，2&lt;=N&lt;=100000，0&lt;=xi&lt;=1000000000</p>

<p>提示：&nbsp;数据十分良心&hellip;&hellip;</p> 
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
<tr><td>5
8 W
11 S
3 W
10 W
5 S</td><td>7</td></tr></table>