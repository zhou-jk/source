# 题目描述


<p class="MsoNormal"><strong>题目描述</strong></p>
<p>很久以前，有一个强大的帝国，它的国土成正方形状，如图 2 2 所示。</p>
<p align="center"><img height="195" width="171" alt="" src="../../mw/images/d/d6/Empire1.jpg"/></p>
<p>这个国家有若干诸侯。由于这些诸侯都曾立下赫赫战功，国王准备给他们每人一块封地</p>
<p>( 正方形中的一格 ) 。但是，这些诸侯又非常好战，当两个诸侯位于同一行或同一列时，他们就会开战。如下图 2-3 为 n=3  时的国土，阴影部分表示诸侯所处的位置。前两幅图中的诸侯</p>
<p>可以互相攻击，第三幅则不可以。</p>
<p><img height="221" width="522" alt="" src="../../mw/images/thumb/f/f2/Xxx3.JPG/800px-Xxx3.JPG"/></p>
<p>国王自然不愿意看到他的诸侯们互相开战，致使国家动荡不安。因此，他希望通过合理的安排诸侯所处的位置，使他们两两之间都不能攻击。</p>
<p>现在，给出正方形的边长 n ，以及需要封地的诸侯数量 k ，要求你求出所有可能的安置方案数。 (n ≤ 100 ， k ≤ 2n 2 -2n+1)</p>
<p>由于方案数可能很多，你只需要输出方案数除以 504 的余数即可。</p>
<p>【输入】</p>
<p>仅一行，两个整数 n 和 k ，中间用一空格隔开</p>
<p>【输出】</p>
<p>一个整数，表示方案数除以 504 的余数。</p>
<p>【样例】</p>
<p>empire.in</p>
<p>2 2</p>
<p>empire.out</p>
<p>4</p>
<p>【样例说明】</p>
<p>四种安置方案如图 2-4 所示。注意：镜面和旋转的情况属于不同的方案。</p>
<p align="center"><img height="179" width="499" alt="" src="../../mw/images/b/b3/Empire2.jpg"/></p>
<p> </p>
