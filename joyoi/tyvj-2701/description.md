# 

 
 # 题目描述 
<p>
<br>幼儿园里有n个小朋友打算通过投票来决定睡不睡午觉。对他们来说，这个问题并不是很重要，于是他们决定发扬谦让精神。虽然每个人都有自己的主见，但是为了照顾一下自己朋友的想法，他们也可以投和自己本来意愿相反的票。我们定义一次投票的冲突数为好朋友之间发生冲突的总数加上和所有和自己本来意愿发生冲突的人数。<br>我们的问题就是，每位小朋友应该怎样投票，才能使冲突数最小？<br><br></p> 

 
 # 输入格式 
<p>
第一行只有两个整数n，m，保证有2≤n≤300，1≤m≤n(n-1)/2。其中n代表总人数，m代表好朋友的对数。文件第二行有n个整数，第i个整数代表第i个小朋友的意愿，当它为1时表示同意睡觉，当它为0时表示反对睡觉。接下来文件还有m行，每行有两个整数i，j。表示i，j是一对好朋友，我们保证任何两对i，j不会重复。<br><br></p> 

 
 # 输出格式 
<p>
只需要输出一个整数，即可能的最小冲突数。<br></p> 

 
 # 提示 
<p>
在第一个例子中，所有小朋友都投赞成票就能得到最优解</p> 
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
<tr><td>3 3
1 0 0
1 2
1 3
3 2
</td><td>1</td></tr></table>
