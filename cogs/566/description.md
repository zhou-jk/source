# 题目描述


<h3>
【问题描述】
</h3>
<p>
圣诞节要来了,有一个舞会.N个男士和N个女士将要参加.一个男士和一个女士成为一对舞伴.我们知道,如果一对舞伴的年龄和身高相差太多的话会不够和协.现在我们定义一个男士和一个女士的不和协值如下: 
</p>
<p>
<br/>
F(i,j)=(Hi-Hj)^2+(AGEi-AGEj)^2<br/>
Hi是i号人员的身高,AGEi是i号人员的年龄.你的任务是设计一个舞伴搭配方案,使最大不合协值最小.
</p>
<h3>
【输入格式】
</h3>
<p>
输入数据第一行为一个正整数N（N≤500），接下来有2N行；
</p>
<p>
每行包含两个正整数x,y，表示身高和年龄（100 ≤x≤200,10≤y≤60）,前N个表示男士,后N个表示女士。
</p>
<h3>
【输出格式】
</h3>
<p>
输出只有一个整数,表示最小的最大不和协值。
</p>
<h3>
【样例输入】
</h3>
<pre>2
141 27
134 10
169 34
178 18
</pre>
<h3>
【样例输出】
</h3>
<pre>1801
</pre>
