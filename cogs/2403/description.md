# 题目描述


<h3>
【问题描述】
</h3>
<p>
 跳蚤国王和蛐蛐国王在玩一个游戏。
</p>
<p>
 他们在一个 n 行 m 列的网格上排兵布阵。其中的 c 个格子中（ 0 ≤ c ≤ nm），每个格子有一只蛐蛐，其余的格子中，每个格子有一只跳蚤。
</p>
<p>
 我们称占据的格子有公共边的两只跳蚤是<strong>相邻</strong>的。
</p>
<p>
 我们称两只跳蚤是<strong>连通</strong>的，当且仅当这两只跳蚤<strong>相邻</strong>，或存在另一只跳蚤与这两只跳蚤都<strong>连通</strong>。
</p>
<p>
 现在，蛐蛐国王希望，将某些（ 0 个， 1 个或多个）跳蚤替换成蛐蛐，使得在此之后存在至少两只跳蚤<strong>不连通</strong>。
</p>
<p>
 例如： 我们用图<img src="/upload/image/20160730/20160730111428_59973.png" alt="(跳蚤)" title="(跳蚤)" align="" height="23" width="30"/>表示一只跳蚤，用图<img src="/upload/image/20160730/20160730111629_39815.png" alt="(蝈蝈)" title="(蝈蝈)" align="" height="31" width="30"/>表示一只蛐蛐，那么图 1 描述了一个 n = 4, m = 4, c = 2 的情况。
</p>
<p>
 这种情况下蛐蛐国王可以通过将第 2 行第 2 列，和第 3 行第 3 列的两只跳蚤替换为蛐蛐，从而达成他的希望，如图 2 所示。并且，不存在更优的方案，但是可能存在其他替换 2 只跳蚤的方案。
</p>
<p>
<img src="/upload/image/20160730/20160730112619_41322.png" alt="" title="" align="" height="225" width="200"/><img src="/upload/image/20160730/20160730112634_97530.png" alt="" title="" align="" height="220" width="203"/> 
</p>
<p>
 你需要首先判断蛐蛐国王的希望能否被达成。如果能够达成，你还需要最小化被替换的跳蚤的个数。
</p>
<h3>
【输入格式】
</h3>
<p>
 每个输入文件包含多组数据。
</p>
<p>
 输入文件的第一行只有一个整数 T，表示数据的组数。 保证 1 ≤ T ≤ 20。
</p>
<p>
 接下来依次输入 T 组数据，每组数据的第一行包含三个整数 n, m, c。 保证 1 ≤ n, m ≤ 10^9， 0 ≤ c ≤ min(nm, 10^5)。
</p>
<p>
 接下来 c 行，每行包含两个整数 x, y，表示第 x 行，第 y 列的格子被一个蛐蛐占据（ 1 ≤ x ≤ n, 1 ≤ y ≤ m）。每一组数据当中，同一个蛐蛐不会被多次描述。
</p>
<p>
 同一行相邻的整数之间由一个空格隔开。
</p>
<h3>
【输出格式】
</h3>
<p>
 对于每一组数据依次输出一行答案。
</p>
<p>
 如果这组数据中，蛐蛐国王的希望不能被达成，输出 -1。否则，输出被替换的跳蚤的个数的最小值。
</p>
<h3>
【样例输入】
</h3>
<pre>4
4 4 2
1 1
4 4
2 3 1
1 2
2 2 2
1 1
2 2
1 1 0 
</pre>
<h3>
【样例输出】
</h3>
<pre>2
1
0
-1
</pre>
<h3>
【样例说明】
</h3>
<p>
 第一组数据就是问题描述中的例子。
</p>
<p>
 对于第二组数据， 可以将第 2 行第 2 列的一只跳蚤替换为蛐蛐，从而使得存在两只跳蚤不连通，并且不存在更优的方案。
</p>
<p>
 对于第三组数据，最初已经存在两只跳蚤不连通，故不需要再进行替换。
</p>
<p>
 对于第四组数据，由于最多只有一只跳蚤，所以无论如何替换都不能存在两只跳蚤不连通。
</p>
<h3>
【更多样例】
</h3>
<p>
<a href="http://pan.baidu.com/s/1bp5dJY3" target="_blank">下载</a> 
</p>
<p>
【样例 2 输入输出】
</p>
<p>
见目录下的 NOI2016grid/NOI2016grid2.in 与 NOI2016grid/NOI2016grid2.ans。
</p>
<h3>
【提示】
</h3>
<p>
如果你的程序需要用到较大的栈空间（这通常意味着需要较深层数的递归），请务必仔细阅读选手目录下的文档 stack.pdf，以了解在最终评测时栈空间的限制与在当前工作环境下调整栈空间限制的方法。
</p>
<p>
PS:来自萌帝的开栈咒语：
</p>
<p>
#pragma comment(linker, &#34;/STACK:102400000,102400000&#34;)
</p>
<h3>
【子任务】
</h3>
<p>
  对于全部的测试点，保证 1 ≤ T ≤ 20。 我们记 ∑c为某个测试点中，其 T 组输入数据的所有 c 的总和。
</p>
<p>
  对于所有的测试点， ∑c ≤ 105。 对于全部的数据，满足 1 ≤ n, m ≤ 10^9, 0 ≤ c ≤ nm, 1 ≤ x ≤ n, 1 ≤ y ≤ m。
</p>
<p>
  每个测试点的详细数据范围见下表。表中的 n, m, c 均是对于单个输入数据 （而非测试点）而言的， 也就是说同一个测试点下的 T 组数据均满足限制条件； 而 ∑c 是对于单个测试点而言的。为了方便阅读，“测试点”一列被放到了表格的中间而不是左边。
</p>
<p>
<img src="/upload/image/20160730/20160730214827_74746.png" alt="" title="" align="" height="732" width="400"/> 
</p>
<h3>
【来源】
</h3>
<p>
NOI2016 Day1 T2
</p>
