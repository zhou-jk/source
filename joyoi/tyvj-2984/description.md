# 

 
 # 题目描述 
<p>
三核苷酸是组成DNA序列的基本片段。具体来说，核苷酸一共有4种，分别用’A’，’G’，’C’，’T’来表示。而三核苷酸就是由3个核苷酸排列而成的DNA片段。三核苷酸一共有64种，分别是’AAA’，’AAG’，…，’GGG’。给定一个长度为L的DNA序列，一共可以分辨出（L-2）个三核苷酸。现在我们想用一些统计学的方法来进行一些分析，步骤如下：

 
 # 输入格式 
<p>
输入包含多组测试数据。第一行包含一个正整数T，表示测试数据数目。每组数据包含一个由’A’，’G’，’C’，’T’组成的字符串，代表要统计的DNA序列。DNA序列的长度大于等于3且不会超过100000。</p> 

 
 # 输出格式 
<p>
对每组测试数据，输出一行答案，为一个保留6位精度的实数，代表S2的值。如果你的答案和标准答案的“相对误差”小于1e-8，你的答案会被视为正确的答案。</p> 
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
<tr><td>1
ATATATA
</td><td>1
ATATATA