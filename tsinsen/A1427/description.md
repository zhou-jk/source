<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　最终，Fox Ciel抵达了她的城堡！<br/>
<br/>
　　她必须输入正确密码才能进入城堡：这个城堡的密码输入端有些与众不同。<br/>
<br/>
　　输入端是一个1*n的长方形，被分成n个小的正方形格子，从左到右依次标号为1~n。每个格子都有开或关两种状态。最初所有的格子都是关闭状态。当且仅当第x1，第x2，...，第xk个格子是打开状态并且其它格子都是关闭状态时，她才能进入城堡。<br/>
<br/>
　　她得到了一个数组a1，...，al。每一步，她可以做如下的操作：选择一个序号i（1 &lt;= i &lt;= l），选择连续的ai个格子，将这些格子的状态取反（即开变关，关变开）。注意，同一个序号可以重复使用。<br/>
<br/>
　　不幸的是，她忘记了如何仅用上述操作来输入密码。请计算输入密码所需的最少操作数。</div>
# 输入格式

<div class="pdcont">　　第一行，包括3个整数n, k, l，之间由空格隔开。<br/>
　　第二行，包括k个整数x1，...,xk(1 &lt;= x1 &lt; x2 &lt; ... &lt; xk &lt;= n)，之间由空格隔开。<br/>
　　第三行，包括l个整数a1, ..., al(1 &lt;= ai &lt;= n)，之间由空格隔开。数组ai中有可能出现重复的元素。</div>
# 输出格式

<div class="pdcont">　　输出仅一行，一个整数，即所需的最少操作数。若不可能正确输入密码，则输出-1。</div>
# 样例输入

<div class="pddata">10 8 2<br/>
1 2 3 5 6 7 8 9<br/>
3 5</div>
# 样例输出

<div class="pddata">2</div>
# 样例输入

<div class="pddata">3 2 1<br/>
1 2<br/>
3</div>
# 样例输出

<div class="pddata">-1</div>
# 数据规模和约定

<div class="pdcont">　　20%的数据满足，1 &lt;= n &lt;= 10.<br/>
　　50%的数据满足，1 &lt;= n &lt;= 100.<br/>
　　100%的数据满足，1 &lt;= n &lt;= 10000, 1 &lt;= k &lt;= 10, 1 &lt;= l &lt;= 100.</div>

</div>