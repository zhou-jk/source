# 题面



<div class="pdcont"><b>问题描述</b><b>   </b><br/>
　　设有N*N的方格图(N&lt;=10),我们将其中的某些方格中填入正整数,而其他的方格中则放入数字0。<br/>
　　某人从图的左上角的A 点(1,1)出发，可以向下行走，也可以向右走，直到到达右下角的B点(N,N)。在走过的路上，他可以取走方格中的数（取走后的方格中将变为数字0）。<br/>
　　此人从A点到B 点共走两次，试找出2条这样的路径，使得取得的数之和为最大。<br/>
<b>输</b><b>入格式</b><br/>
　　输入的第一行为一个整数N（表示N*N的方格图），接下来的每行有三个整数，前两个表示位置，第三个数为该位置上所放的数。一行单独的0表示输入结束。<br/>
<b>输</b><b>出格式</b><br/>
　　只需输出一个整数，表示2条路径上取得的最大的和。<br/>
<b>样</b><b>例</b><b>输</b><b>入</b><br/>
　　8<br/>
　　2 3 13<br/>
　　2 6 6<br/>
　　3 5 7<br/>
　　4 4 14<br/>
　　5 2 21<br/>
　　5 6 4<br/>
　　6 3 15<br/>
　　7 2 14<br/>
　　0 0 0<br/>
<b>样例输出</b><br/>
　　67</div>



