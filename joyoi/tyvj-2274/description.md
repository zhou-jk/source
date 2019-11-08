# 

 
 # 题目描述 
<p>
波罗的海的考古学家最近正参与一个非常重要的工程，并发现了一个古老的手稿 ，这个手稿对于理解他们正在探索区域的居民文化起着关键性的作用。手稿上主要由图案构成, 因此考古学家能够对文档的主题有个大致的概念。 

 
 # 输入格式 
<p>
 The first line of the input file contains four integers VE, VC, CE and CC (1 ≤ VE ≤ VC ≤ 4, 1 ≤ CE ≤ CC ≤ 4) separated by single spaces. 第二行描述一个从手稿中抽出的单词，它由最多15个英文小写单词构成，如果某一位为“*”，那么说明这个字母已经模糊不清了。

 
 # 输出格式 
<p>
 输出只有一个整数，描述有多少种可能的合法单词符合上文给出的限制条件。你可以假设答案不超过64位带符号的整数。有可能那位考古学家的假设是错误的，不存在任何一种可能的合法单词，那么答案输出为0。
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
<tr><td>1 1 1 1
a**
</td><td>105</td></tr></table>