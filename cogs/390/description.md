# 题目描述


<p>小 Y 太失败了，他虽然在化学实验课上拿来了很多溶液，但是还是没有办法配成想要的溶液，万一倒错了就没有办法挽回了，小 Y 迟迟不敢下手。</p>
<p>于是小 Y 到网上下载了一个溶液配置模拟器。溶液配置模拟器是这样的程序：模拟器在电脑中构造一种虚拟溶液，然后你可以虚拟地向当前虚拟溶液中加入一定浓度一定质量的这种溶液，模拟器会快速地算出倒入后虚拟溶液的浓度和质量。当然，计算机最可爱的地方就是当你倒错了可以撤销。</p>
<p>模拟器的使用步骤是这样的：</p>
<p>1. 为模拟器设置一个初始质量和浓度 V0 ， C0% （ 0 ≤ C0≤100 ）。</p>
<p>2. 进行一系列操作，模拟器支持两种操作：</p>
<p>P(v,c) 操作：表示向当前的虚拟溶液中加入质量为 v 浓度为 c 的溶液；</p>
<p>Z 操作：撤销上一步 P 操作。</p>
<p>但是，小 Y 不小心把模拟器弄丢了……，眼看考试迫在眉睫，小 Y 只能依靠你了。</p>
<p>输入格式：</p>
<p>第一行，两个整数 V0 ， C0 。</p>
<p>第二行，一个整数 n ，表示操作数（ n ≤ 10000 ）。</p>
<p>接下来 n 行，每行一条操作，格式为：</p>
<p>P v c 或 Z 。</p>
<p>之间用一个空格隔开，当只剩初始溶液的时候，再撤销就没有用了。</p>
<p>任意时刻质量不会超过 2 31 -1 。</p>
<p>输出格式：</p>
<p>n 行，每行两个数 V i ， C i , 其中 V i 为整数， C i 为实数（保留 5 位小数），之间用一个空格隔开。其中，第 i 行表示第 i 次操作以后的溶液质量和浓度。</p>
<p>输入样例：</p>
<p>100 100</p>
<p>2</p>
<p>P 100 0</p>
<p>Z</p>
<p>输出样例：</p>
<p>200 50.00000</p>
<p>100 100.00000</p>
