# 题目描述


<h3>
【题目描述】
</h3>
<p>
小F有一个梦想：为数列写一个最强大的编辑器！ 一开始，数列为空，光标在开头位置，小F的编辑器要对这个数列作如下五种操作：
</p>
<p>
I x：在光标的后面插入一个数字x，并将光标移到这个新加入的x后。
</p>
<p>
D：删除光标前的最后一个数字（保证存在），光标位置不变。
</p>
<p>
L：光标左移一位，如果已经在开头则不做任何事。
</p>
<p>
R：光标右移一位，如果已经在结尾则不做任何事。
</p>
<p>
Q k：编辑器需要给出A1 A2 ··· Ak的最大前缀和（前缀长度不能为0），保证1 ≤ k ≤ N，其中N为当前光标前的数字个数。
</p>
<p>
<br/>
</p>
<h3>
【输入格式】
</h3>
<p>
<br/>
</p>
<p>
第一行，一个整数Q，表示操作的总次数。
</p>
<p>
后Q行，每行是上列五种操作中的一种。
</p>
<p>
<br/>
</p>
<p>
<br/>
</p>
<h3>
【输出格式】
</h3>
<p>
<br/>
</p>
<p>
对每个Q操作，输出一行一个整数，表示答案。
</p>
<p>
<br/>
</p>
<p>
<br/>
</p>
<h3>
【样例输入】
</h3>
<p>
8
</p>
<p>
I 2
</p>
<p>
I -1
</p>
<p>
I 1
</p>
<p>
Q 3
</p>
<p>
L
</p>
<p>
D
</p>
<p>
R
</p>
<p>
Q  22
</p>
<p>
2
</p>
<h3>
【样例输出】
</h3>
<p>
2
</p>
<p>
3
</p>
<h3>
【样例解释】
</h3>
<p>
<br/>
</p>
<p>
每次操作的结果如下（其中|表示光标位置）：
</p>
<p>
I 2：[2|]
</p>
<p>
I −1：[2 −1|]
</p>
<p>
I 1：[2 −1 1|]
</p>
<p>
Q 3：[2 −1 1|]，前3个数的最大前缀和为2
</p>
<p>
L：[2 −1|1]
</p>
<p>
D：[2|1]
</p>
<p>
R：[2 1|]
</p>
<p>
Q 2：[2 1|]，前2个数的最大前缀和为3
</p>
<p>
<br/>
</p>
<p>
<br/>
</p>
<h3>
【数据范围及提示】
</h3>
<p>
</p><table style="width:100%;" border="1" bordercolor="#000000" cellpadding="2" cellspacing="0">
<tbody>
<tr>
<td>
测试点编号                                           <br/>
</td>
<td>
 包含操作种类<br/>
</td>
<td>
Q<br/>
</td>
<td>
X<br/>
</td>
</tr>
<tr>
<td>
1<br/>
</td>
<td>
I    Q<br/>
</td>
<td>
10<br/>
</td>
<td>
【-1，1】<br/>
</td>
</tr>
<tr>
<td>
2<br/>
</td>
<td>
I    Q<br/>
</td>
<td>
500000<br/>
</td>
<td>
【-1000，1000】<br/>
</td>
</tr>
<tr>
<td>
3<br/>
</td>
<td>
I    Q<br/>
</td>
<td>
1000000
</td>
<td>
同上<br/>
</td>
</tr>
<tr>
<td>
4<br/>
</td>
<td>
I    D    L    R     Q<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
5                                                                                                <br/>
</td>
<td>
<p>
<br/>
</p>
<p>
同上
</p>
<p>
<br/>
</p>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
6<br/>
</td>
<td>
<p>
同上
</p>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
7<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
8<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
9<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
10<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
11<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
12<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
13<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
14<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
15<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
16<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
17<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
18<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
19<br/>
</td>
<td>
同上<br/>
</td>
<td>
100000<br/>
</td>
<td>
...<br/>
</td>
</tr>
<tr>
<td>
20<br/>
</td>
<td>
同上<br/>
</td>
<td>
1000000<br/>
</td>
<td>
...<br/>
</td>
</tr>
</tbody>
</table>
<p></p>
