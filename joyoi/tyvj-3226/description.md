# 

 
 # 题目描述 
<p>
会议中心（CONVENTION.cpp/c/pas）<br><br>【问题描述】<br><br>　　Siruseri政府建造了一座新的会议中心。许多公司对租借会议中心的会堂很感兴趣，他们希望能够在里面举行会议。 对于一个客户而言，仅当在开会时能够独自占用整个会堂，他才会租借会堂。会议中心的销售主管认为：最好的策略应该是将会堂租借给尽可能多的客户。显然，有可能存在不止一种满足要求的策略。 例如下面的例子。总共有4个公司。他们对租借会堂发出了请求，并提出了他们所需占用会堂的起止日期（如下表所示）。<br><br><center><img src="/source/joyoi/tyvj-3226/img/aHR0cDovL3d3dy5qb3lvaS5jbi9wcm9ibGVtL3R5dmotMzIyNi9wcm9ibGVtc19pbWFnZXMvMTczOC9wMS5naWY=.gif"></img></center><br>　　上例中，最多将会堂租借给两家公司。租借策略分别是租给公司1和公司3，或是公司2和公司3，也可以是公司1和公司4。注意会议中心一天最多租借给一个公司，所以公司1和公司2不能同时租借会议中心，因为他们在第九天重合了。<br>销售主管为了公平起见，决定按照如下的程序来确定选择何种租借策略：首先，将租借给客户数量最多的策略作为候选，将所有的公司按照他们发出请求的顺序编号。对于候选策略，将策略中的每家公司的编号按升序排列。最后，选出其中字典序最小1的候选策略作为最终的策略。 例中，会堂最终将被租借给公司1和公司3：3个候选策略是{(1,3),(2,3),(1,4)}。而在字典序中(1,3)<(1,4)<(2,3)。 你的任务是帮助销售主管确定应该将会堂租借给哪些公司。<br></p> 

 
 # 输入格式 
<p>
　　输入的第一行有一个整数N，表示发出租借会堂申请的公司的个数。第2到第N+1行每行有2个整数。第i+1行的整数表示第i家公司申请租借的起始和终止日期。对于每个公司的申请，起始日期为不小于1的整数，终止日期为不大于109的整数。</p> 

 
 # 输出格式 
<p>
　　输出的第一行应有一个整数M，表示最多可以租借给多少家公司。第二行应列出M个数，表示最终将会堂租借给哪些公司。</p> 

 
 # 提示 
<p>
　　对于50%的输入，N≤3000。在所有输入中，N≤200000。</p> 
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
4 9
9 11
13 19
10 17
</td><td>2
1 3</td></tr></table>
