# 题目描述


<p>
【问题描述】
</p>
<p>
本题中，我们考察的是一类特殊的序列，这类序列只有+、-（正号，负号）两种符号构成，比如：-+++---++
</p>
<p>
我们将其中连续的+的长度按从左到右的顺序写出，即其派生序列，如-+++---++的派生序列为（3，2）。
</p>
<p>
现在的问题是，我们已知一个序列A的派生序列B，但是A的部分符号已经模糊到不能辨认的地步了。我们需要确定尽量多的符号。
</p>
<p>
<br/>
</p>
<p>
【输入文件】
</p>
<p>
输入文件有两行。
</p>
<p>
第一行一个由+、-、？构成的序列，描述A，其中？表示已经无法辨认的符号。
</p>
<p>
第二行有若干整数描述A的生成序列B。
</p>
<p>
<br/>
</p>
<p>
【输出文件】
</p>
<p>
输出一行，一个序列描述你恢复后的序列A（不能多余的空格），如果无解则输出一行No Solution。
</p>
<p>
<br/>
</p>
<p>
【数据约定】
</p>
<p>
对于30%的数据满足|A| &lt; 11
</p>
<p>
对于50%的数据满足|A| &lt; 101
</p>
<p>
对于100%的数据满足|A| &lt; 20001
</p>
<p>
B的元素属于[1 … |A|]
</p>
<p>
<br/>
</p>
<p>
【样例】
</p>
<p>
输入样例1
</p>
<p>
+-?+-+++
</p>
<p>
1 2 3
</p>
<p>
输出样例1
</p>
<p>
+-++-+++
</p>
<p>
输入样例2
</p>
<p>
???
</p>
<p>
2
</p>
<p>
输出样例2
</p>
<p>
?+?
</p>
<p>
输入样例3
</p>
<p>
--
</p>
<p>
1
</p>
<p>
输出样例3
</p>
<p>
No Solution
</p>
