# 

 
 # 题目描述 
<p>
　　我们都很熟悉二叉树的前序、中序、后序遍历，在数据结构中常提出这样的问题：已知一棵二叉树的前序和中序遍历，求它的后序遍历，相应的，已知一棵二叉树的后序遍历和中序遍历序列你也能求出它的前序遍历。然而给定一棵二叉树的前序和后序遍历，你却不能确定其中序遍历序列，考虑如下图中的几棵二叉树：

 
 # 输入格式 
<p>
　　输A数据共两行，第一行表示该二叉树的前序遍历结果s1，第二行表示该二叉树的后序遍历结果s2。</p> 

 
 # 输出格式 
<p>
　　输出可能的中序遍历序列的总数，结果不超过长整型数。</p> 

 
 # 提示 
<p>
【算法分析】
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
<tr><td>abc						
bca
</td><td>4</td></tr></table>