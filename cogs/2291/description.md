# 题目描述


<h3>
【题目描述】
</h3>
<p>
本蒟蒻特别喜欢吃火龙果
</p>
<p>
听说某魔法学院的火龙果吃了之后能变成大火龙
</p>
<p>
于是本蒟蒻兴致勃勃的来到了魔法学院来寻找这神奇的火龙果
</p>
<p>
在魔法学院，本蒟蒻发现如果想要吃到火龙果，就必须学习魔法来解除禁制
</p>
<p>
<br/>
</p>
<p>
已知魔法世界一共有n种元素，本蒟蒻会m种魔法
</p>
<p>
每种魔法可以使得本蒟蒻把u元素转化为v元素，也可以使得本蒟蒻把v元素转化为u元素
</p>
<p>
但是每种魔法都对本蒟蒻的生命值，魔法值和等级有要求，每种魔法有三种属性A,B,C
</p>
<p>
当且仅当本蒟蒻的生命值&gt;=A且本蒟蒻的魔法值&gt;=B且本蒟蒻的等级&gt;=C的时候才能施展该魔法
</p>
<p>
注意由于本蒟蒻的魔法学得还不错，所以施展任何魔法并不会消耗生命值或者魔法值或者等级
</p>
<p>
现在本蒟蒻想知道当他的生命值为D且魔法值为E的时候想要完成u元素到v元素的转化需要的最小等级是多少
</p>
<p>
如果无论本蒟蒻的等级多高，都不能完成u元素到v元素的转化，则输出-1
</p>
<h3>
【输入格式】
</h3>
<p>
第一行输入n,m,q 代表元素种类，本蒟蒻会的魔法数量和询问次数
</p>
<p>
以下m行，每行描述一个魔法，输入u，v，A，B，C 含义如题意所示
</p>
<p>
以下q行，每行描述一个询问，输入u，v，D，E 含义如题意所示
</p>
<p>
n,m,q&lt;=30000,A,B,C&lt;=10000
</p>
<p>
保证不存在u元素转化成自身的魔法
</p>
<h3>
【输出格式】
</h3>
<p>
对于每个询问输出相应的答案
</p>
<h3>
【样例输入】
</h3>
<pre><p>
3 3 3
</p>

<p>
1 2 2 2 3
</p>

<p>
1 3 2 3 2
</p>

<p>
2 3 1 1 1
</p>

<p>
1 2 2 2
</p>

<p>
1 2 3 3
</p>

<p>
1 2 2 1
</p>

<p>
<br/>

</p>
</pre>
<h3>
【样例输出】
</h3>
<pre><p>
3
</p>

<p>
2
</p>

<p>
-1<span style="font-family:monospace;"></span> 
</p>

<p>
<br/>

</p>

<p>
样例解释：
</p>

<p>
对于第一个询问，只能从1-&gt;2 需要等级为3
</p>

<p>
对于第二个询问，有两种方案
</p>

<p>
第一种1-&gt;2 需要等级为3
</p>

<p>
第二种1-&gt;3-&gt;2 需要等级分别为2,1 因为需要完成整个转化，所以这个方案的最小等级为2
</p>

<p>
对于两种方案取最小值，需要等级为2
</p>

<p>
对于第三个询问，显然不存在1转化为2的方案，输出-1
</p>

<p>
评测请开启O2优化
</p>
</pre>
