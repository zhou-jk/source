# 题目描述


<p>
问题描述
</p>
<p>
一棵二叉树可以按照如下规则表示成一个由0、1、2组成的字符序列，我们称之为“二叉树序列S”：
</p>
<ul>
<li>
0 该树没有子节点
</li>
<li>
1S1 该树有一个子节点，S1为其二叉树序列
</li>
<li>
1S1S2 该树有两个子节点，S1,S2分别为两个二叉树的序列
</li>
</ul>
<p>
例如，下图所表示的二叉树可以用二叉树序列S=21200110来表示。
</p>
<p>
<span><img width="231" height="128" alt="Image:Trot.gif" src="../../mw/images/5/52/Trot.gif"/></span> 
</p>
<p>
你的任务是要对一棵二叉树的节点进行染色。每个节点可以被染成红色、绿色或蓝色。并且，一个节点与其子节点的颜色必须不同，如果该节点有两个子节点，那么这两个子节点的颜色也必须不相同。给定一棵二叉树的二叉树序列，请求出这棵树中最多和最少有多少个点能够被染成绿色。
</p>
<p>
输入文件
</p>
<p>
<br/>
输入文件仅有一行，不超过10000个字符，表示一个二叉树序列。
</p>
<p>
输出文件
</p>
<p>
输出文件也只有一行，包含两个数，依次表示最多和最少有多少个点能够被染成绿色。
</p>
<p>
样例输入
</p>
<p>
1122002010
</p>
<p>
样例输出
</p>
<p>
5 2
</p>
