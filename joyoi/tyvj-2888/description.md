# 

 
 # 题目描述 
<p>
话说3008年的Orz教主节，全民狂欢，传递教主圣火，以致万人空巷，股票飞涨。真乃锣鼓喧天，鞭炮齐鸣，红旗招展，人山人海呐。可是小X为了准备NOIP3008，不得不待在家里好好Coding。小X希望早点结束当天的任务，加入圣火传递队伍中去。<br>在这个不亚于狂欢节的日子里，小X的老师却“公然违抗”休假法令，布置小X写一个小根堆，但是小X不会堆的操作，所以想了一个偷懒的办法：<br>堆是一棵完全二叉树，每个结点有一个权。小根堆的根的权最小，且根的两个子树也是一个堆。可以用一个数组a来记录一棵完全二叉树，a[1]为根结点，若结点a[j]不是根结点，那么它的父亲为a[j/2]（取下整）；若结点a[k]不是叶子结点，那么它的左儿子为a[2k]，它的右儿子为a[2k+1]。<br>他希望一组数据按一定顺序依次插入数组中（即第i个数为a[i]），最后得出来就已经是一个堆，即不需要任何交换操作，若有多种方法，输出字典序最大的一组，显得这个数据更乱。<br></p> 

 
 # 输入格式 
<p>
输入的第1行为一个正整数n，为插入的数字的个数。<br>第2行包含n个正整数，为所有需要插入的数字，数字之间用空格隔开。<br>为了简化题目，数据保证n=2^k-1，即保证最后的堆是一棵满二叉树。<br></p> 

 
 # 输出格式 
<p>
输出包括1行，为插入的序列，数字之间用空格隔开，行末换行并没有空格。</p> 

 
 # 提示 
<p>
【样例说明】<br>1 2 10与1 10 2都是满足要求的插入序列，但是1 10 2的字典序更大。<br><br>【数据规模】<br>对于20%的数据，n≤7；<br>对于30%的数据，n≤15；<br>对于50%的数据，n≤1023； <br>对于100%的数据，n≤65535，所有数字不超过10^8，且各不相同。<br><br></p> 
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
<tr><td>3
10 2 1
</td><td>1 10 2</td></tr></table>
