# 题目描述

<p>最近傲娇少女幽香很忙，于是让跳蚤国王出了一道题给 ZJOI2015，一时间人人自危。你秘密潜伏了下来想窃取跳蚤国王的试题。</p>
<p>终于有一天，趁跳蚤国王出去练习跳高，你偷偷打开了跳蚤国王的电脑 —— 结果发现试题被 $10$ 个电子密码锁锁住了！</p>
<p>任何事情都阻挡不了你进省队的决心！每个电子密码锁内部有 $10$ 道检测工序，输入密码后，每通过一道检测工序密码锁就会输出一行 “<samp>ok</samp>”。如果输出了 $10$ 行 “<samp>ok</samp>” 那么就解开了该密码锁。</p>
<p>根据常识知，跳蚤国王一定是用高级计算机语言 <samp>flea++</samp> 写代码的，然后用 <samp>flea++</samp> 的编译器编译成汇编代码，再用汇编编译器编译为机器码。</p>
<p>显然你没有这 $10$ 个电子密码锁的 <samp>flea++</samp> 源代码，通过反汇编，你获得了这 $10$ 个电子密码锁的汇编代码。</p>
<p>跳蚤的程序开始运行时会开出长度为 $2^{23}$ 的 $32$ 位有符号整数数组 $a$，元素分别为 $a_0, a_1, \dots, a_{2^{23} - 1}$，并全部初始化为 $0$。</p>
<p>在跳蚤的汇编语言中，有三种量：“<samp>@ $c$</samp>”，“<samp>\$ $c$</samp>”，“<samp># $c$</samp>” （不含引号）。其中 $c$ 是个整数且 $c \in [-2^{31}, 2^{31})$。</p>
<ul><li>“<samp>@ $c$</samp>” 表示整数常量 $c$。</li>
<li>“<samp>\$ $c$</samp>” 表示 $a_c$。</li>
<li>“<samp># $c$</samp>” 表示 $a_{a_c}$。</li>
</ul><p>如果程序运行过程中试图访问的量会导致数组下标越界，那么就会产生 “<samp>Runtime Error</samp>” 错误并异常退出。</p>
<p>汇编代码由若干行组成，每行是一条语句（从 $1$ 开始编号），程序会从第 $1$ 条语句从上往下执行。</p>
<p>语句有下面这么几种：</p>
<ul><li>赋值语句：<samp>= $a$ $b$</samp><ul><li>$a, b$ 是某个量。</li>
<li>表示把 $b$ 的值赋给 $a$。</li>
<li>如果 $a$ 是个整数常量那么会产生 <samp>Runtime Error</samp> 错误并异常退出。</li>
</ul></li>
<li>输入语句：<samp>getc $c$</samp> 和 <samp>geti $c$</samp><ul><li>$c$ 是某个量。</li>
<li><samp>getc $c$</samp> 表示读入一个字符，把该字符的 <samp>ASCII</samp> 码存入 $c$ 中。</li>
<li><samp>geti $c$</samp> 表示读到下一个非空白字符的位置，读入十进制表示的 $32$ 位有符号整数，存入 $c$ 中。（空白字符即 <samp>ASCII</samp> 码为 $9, 10, 13, 32$ 的字符）</li>
<li>如果 $c$ 是个整数常量那么会产生 <samp>Runtime Error</samp> 错误并异常退出。如果读入整数失败则输出相关信息并异常退出。</li>
</ul></li>
<li>输出语句：<samp>putc $c$</samp> 和 <samp>puti $c$</samp><ul><li>$c$ 是某个量。</li>
<li><samp>putc $c$</samp> 表示输出一个字符，$c$ 是该字符的 <samp>ASCII</samp> 码。</li>
<li><samp>puti $c$</samp> 表示输出整数 $c$ 的十进制表示。</li>
</ul></li>
<li>条件跳转语句：<samp>if $c$ $t$</samp><ul><li>$c, t$ 是某个量。</li>
<li>表示如果 $c$ 不是 $0$，那么跳转到第 $t$ 条语句继续执行（即下一条要执行的语句变为第 $t$ 条语句）；</li>
<li>如果是 $0$，那么不进行任何操作，继续执行下一条语句。</li>
</ul></li>
<li>运算语句：<samp>$o$ $a$ $b$ $c$</samp><ul><li>$a, b, c$ 是某个量，$o$ 是某个运算符。</li>
<li>该语句表示把 $a$ 和 $b$ 进行 $o$ 的运算，把结果赋值给 $c$。</li>
<li>如果 $o$ 是 <samp>+</samp> 则表示加法，即 $a + b$。</li>
<li>如果 $o$ 是 <samp>-</samp> 则表示减法，即 $a - b$。</li>
<li>如果 $o$ 是 <samp>*</samp> 则表示乘法，即 $a \times b$。</li>
<li>如果 $o$ 是 <samp>/</samp> 则表示做除法然后下取整，即 $\lfloor \frac{a}{b} \rfloor$。</li>
<li>如果 $o$ 是 <samp>&lt;</samp> 则表示 $a &lt; b$ 则结果为 $1$，否则为 $0$。</li>
<li>如果 $o$ 是 <samp>==</samp> 则表示 $a = b$ 则结果为 $1$，否则为 $0$。</li>
<li>如果 $c$ 是个整数常量或者作除法时除数为 $0$ 那么会产生 <samp>Runtime Error</samp> 错误并异常退出。</li>
</ul></li>
</ul><p>程序运行过程中如果试图执行第 $-1$ 条语句那么程序正常结束，如果试图执行除此之外的不存在的语句那么会产生 <samp>Runtime Error</samp> 错误并异常退出。</p>
<p>如果执行的语句条数超过 $10^7$ 那么会产生 <samp>Time Limit Exceeded</samp> 错误并异常退出。</p>
<p>现在，是时候展现你卓越的黑客技术了！</p>
# 输入格式


<p>本题为提交答案题。所有输入数据 <samp>lock1.in～lock10.in</samp> 见数据下载。</p>
<p>每个输入文件表示一个密码锁的汇编代码。</p>
<p>我们还提供了一个来自跳蚤国的模拟器，能直接执行汇编代码。</p>
<p>在终端中先切换到该试题的目录下（Windows 选手请使用 <samp>cmd</samp>）。</p>
<p>然后在终端中运行：<samp>./run_linux64 &lt;code&gt;</samp>。其中 <samp>&lt;code&gt;</samp> 是你要执行的汇编代码的文件名。例如：<samp>./run lock1.in</samp>（当然我们也提供了对应的 32 位版本 <samp>run_linux32</samp>，Windows 选手请使用 <samp>run_win32 lock1.in</samp>）</p>
<p>模拟器将从终端中读入数据。如果你想从文件中读入，请使用 <samp>&lt;</samp> 来指定。</p>
<p>例如：<samp>./run lock1.in &lt;lock1.out</samp></p>
<p>其它操作系统请安装 <a href="http://nodejs.org/download/">node.js</a> 然后使用 <samp>node run.js &lt;code&gt;</samp> 运行。</p>
# 输出格式


<p>针对给定的 $10$ 个输入文件 <samp>lock1.in～lock10.in</samp>，你需要分别给出你的输出文件 <samp>lock1.out～lock10.out</samp>。</p>
<p>每个输出文件包含一些字符，表示你输入的密码。</p>
# 样例一


<h4>input</h4>
<pre>= $ 4 @ 8388607
= # 4 @ -1
- $ 4 @ 1 $ 4
if @ 1 @ 5
= # 4 $ 5
- $ 4 @ 1 $ 4
= $ 5 $ 4
- $ 4 @ 1 $ 4
- $ 4 @ 1 $ 4
geti $ 0
= # 4 $ 0
- $ 4 @ 1 $ 4
+ $ 5 @ 0 $ 0
+ $ 4 @ 1 $ 4
= $ 1 # 4
= # 0 $ 1
+ $ 5 @ 0 $ 0
= # 4 $ 0
- $ 4 @ 1 $ 4
+ $ 4 @ 1 $ 4
= $ 1 # 4
== # 1 @ 666 $ 0
if $ 0 @ 25
if @ 1 @ 41
+ $ 5 @ -1 $ 0
= # 0 @ 0
if @ 1 @ 34
putc @ 111
putc @ 107
putc @ 10
+ $ 5 @ -1 $ 0
+ # 0 @ 1 # 0
- # 0 @ 1 $ 0
+ $ 5 @ -1 $ 0
= # 4 $ 0
- $ 4 @ 1 $ 4
+ $ 4 @ 1 $ 4
= $ 1 # 4
&lt; # 1 @ 10 $ 0
if $ 0 @ 28
= $ 0 @ 0
+ $ 4 @ 2 $ 4
= $ 4 $ 5
+ $ 4 @ 1 $ 4
= $ 5 # 4
+ $ 4 @ 1 $ 4
if @ 1 # 4

</pre>

<h4>output</h4>
<pre>666

</pre>

<h4>explanation</h4>
<p>该程序会读入一个整数，如果这个整数是 $666$ 那么就会输出 $10$ 行 “<samp>ok</samp>”。</p>
# 评分方式


<p>每个密码锁为一个测试点，每个测试点 $10$ 分。</p>
<p>对于每个密码锁，我们会以你的输出文件作为输入运行密码锁。</p>
<p>如果程序异常退出则该测试点 $0$ 分。</p>
<p>否则，我们会检查密码锁输出的每一行，设有 $x$ 行为 “<samp>ok</samp>”。如果 $x \geq 10$ 则该测试点满分，否则该测试点得 $x$ 分。</p>
# 后记


<p>你花了很长时间破解密码锁，最后也没有破解出来。最后硬着头皮去了 ZJOI2015,发现自己的事迹被写在了题面里。</p>
# 备注


<p>题目中提到的 “$32$ 位有符号整数” 等价于 <samp>C/C++</samp> 中的 <samp>int</samp>，<samp>Pascal</samp> 中的 <samp>longint</samp>，能表示 $[-2^{31}, 2^{31})$ 以内的整数。</p>
<p>计算过程可能会溢出，比如：$2147483647 + 1 = -2147483648$，$100000 \times 100000 = 1410065408$。</p>
# 下载


<p><a href="/download.php?type=problem&amp;id=116">数据下载</a></p>