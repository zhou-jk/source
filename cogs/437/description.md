# 题目描述


<p>
连通图是指任意两个顶点都有路径可互相到达的图。<br/>
读入一个无向的连通图，输出最多能删掉多少条边，使这个图仍然连通。
</p>
<div>
<b>【</b>输入格式】
</div>
<div>
第1行为图的顶点数N(1≤N≤100)和边数M，它们之间用一个空格隔开，图中的顶点用1到N的整数标号。接下来的M行，每行用两个数V<sub>1</sub>，V<sub>2</sub>和也表示一边条。V<sub>1</sub>与V<sub>2</sub>用一个空格隔开，表示这条边所连接的顶点的标号(V<sub>1</sub>&lt;&gt;V<sub>2</sub>)，同一条边不会重复出现。
</div>
<div>
<b>【</b>输出格式】
</div>
<div>
输出最多能删掉的边数。
</div>
<div>
<b>【</b>输入输出样例】<br/>
输 入(edges.in)<br/>
5 7<br/>
4 6<br/>
1 2<br/>
1 3<br/>
1 4<br/>
2 3<br/>
2 4<br/>
3 4<br/>
输 出(edges.out)<br/>
3
</div>
