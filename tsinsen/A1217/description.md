<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　平行宇宙，或者叫做多重宇宙论，这是一种在物理学里尚未被证实的理论。<br/>
　　我们假想，在某个事件点(以时间为轴)之后，宇宙的运行轨迹会出现许多可能，而这些可能的宇宙是平行的。举例来说，从我们现在存在的这个宇宙开始，每过一个时刻，宇宙就会分成很多个，在这些宇宙中，会有成为警察的你，会有成为总理的你，等等。而这些不同的宇宙是相互平行的，且在之后的发展中也是平行，不会相交。<br/>
　　现在我们进入正题。<br/>
　　我们正在使用计算机读数据，数据有K行，每行一个非负整数。我们需要按如下方式读取数据:<br/>
　　1、首先读入第一个数，需要支付1的代价。<br/>
　　2、我们假设读入的数是x，那么我们需要读入接下来x个数。<br/>
　　3、如果文件已经读完，则读入结束；否则我们接着再读一个数(需要支付$1$的代价)，然后转2。<br/>
　　数据保证任何一个读入的x，在他后面至少还有x个数字。虽然按照上面的方法一定可以恰好读完数据，但是这么做支付的代价不一定是最小的，你可以<br/>
　　修改读入的那个x，可以把x修改为x+y或者x-y，不过必须保证，值仍然是非负整数，且接下来有不少于x±y个数。<br/>
　　而我们需要支付的代价就是y。<br/>
　　相信你已经猜到我们的问题了，那就是恰好读完所有数据，需要支付的最少代价是多少。<br/>
　　等等，似乎还缺了什么。没错，我们并不知道这些数据是什么，但我们知道这些数据可能是什么，就像薛定谔的猫。在没有读入这个数字之前，它什么都是，<br/>
　　一旦读入了这个数，根据结果，我们就进入了不同的平行世界。<br/>
　　现在我将告诉你宇宙可能出现的轨迹，希望你计算出所有不同的结果(读完数据需要支付的最小代价)。</div>
# 输入格式

<div class="pdcont">　　为了方便起见，我们把读入一个数看成一个事件，我们用1 … N把所有可能的事件编号。<br/>
　　第一行，读入一个整数N，表示可能的事件的个数。<br/>
　　接下来N行，第i+1行描述第i个事件。第i个事件，将会告知这些参数x m a1 a2 a3 … ：<br/>
　　x 表示第$i$个事件的数据值是多少。<br/>
　　m 表示这个事件之后有多少种可能出现的事件，编号是a1 a2 a3 …。<br/>
　　其中第1个事件，它的数据值一定是-1，因为这时第一个数还未读入。也就是说，第1个事件所相关的事件a1 a2 a3 …，就是读入的第一个数所有的可能值。且如果某个事件m=0，那么这个所读入的数x，就是数据中的最后一个数。</div>
# 输出格式

<div class="pdcont">　　输出M行，M是最终所有可能的不同宇宙的个数。<br/>
　　每行输出一个最小的代价值，按照代价值的大小，从小到大输出。</div>
# 样例输入

<div class="pddata">7<br/>
-1 1 2<br/>
1 2 3 7<br/>
3 1 4<br/>
0 1 5<br/>
0 1 6<br/>
0 0<br/>
0 0</div>
# 样例输出

<div class="pddata">1<br/>
3</div>
# 数据规模和约定

<div class="pdcont">　　数据保证有20% 的数据N≤2000；<br/>
　　保证有60%的数据N≤200000；<br/>
　　另有20%的数据，输出的个数M ≤50。<br/>
　　所有数据N≤1000000。</div>

</div>