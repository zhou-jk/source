# 

 
 # 题目描述 
&nbsp;&nbsp;&nbsp;&nbsp;刘老师给他教的小学生们出了一些题目，测试他们计算加法、减法和乘法的<BR>能力。为了让阅卷尽量简单，他故意使所有题目的答案都等于2000（小孩子一般<BR>不会发现这个规律的吧）。当它把试卷打印出来以后发现了一个严重的问题：所<BR>有的符号都不见了（电脑病毒？），更可恶的是，题目的电子版也不见了，现在<BR>只能从残缺的题目中恢复原来的数据。例如“2100100=”可能是“2100-100=”，<BR>“2*100*10+0=”，“2*100*10-0=”，“2*10*0100=”，“2*-100*-10+0=”中的<BR>一个。<BR>但是刘老师强调，他出题的规则是：<BR>1.只用二元+，-，*三种符号，没有括号，也没有一元运算（即+不能做正<BR>号，-也不能做负号）。因此“2*-100*-10+0=”是不合法的。<BR>2.不写以0开头的正数；如果这个数是0则只会写一个0而不是000这样的奇怪<BR>形式。<BR>3.运算符合通常的运算顺序和结合性（先乘法，后加减法，左结合）<BR>因此合法的解只有三个。如果有多种可能，按照任何顺序输出均可。<BR> 

 
 # 输入格式 
&nbsp;&nbsp;&nbsp;&nbsp;输入文件op.in仅包含一行，为丢失符号后的表达式，即不超过9个0~9的<BR>数字后跟一个“=”号。 

 
 # 输出格式 
&nbsp;&nbsp;&nbsp;&nbsp;输出文件op.out包含若干行，每行包含一个合法的问题。如果无解，<BR>输出“NO”。 

 
 # 提示 
SCOI2004&nbsp;day1&nbsp;T3 
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
<tr><td>样例1:

2100100=

样例2：

77=

</td><td>样例1:

2100-100=
2*100*10+0=
2*100*10-0=

样例2：

NO
</td></tr></table>
