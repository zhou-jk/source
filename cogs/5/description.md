# 题目描述


<p>
 <b>问题描述</b><br/>
<span style="font-size:10.5pt;"><span style="font-size:10.5pt;">为了进一步普及九年义务教育，政府要在某乡镇建立P所希望小学，该乡镇共有n个村庄，村庄间的距离已知，请问学校建在哪P个村庄最好？（好坏的标准是学生就近入学，即在来上学的学生中，以最远的学生走的路程为标准。或者说最远的学生与学校的距离尽可能的小。）</span></span> 
</p>
<div align="center">
 <img alt="" src="/images/fwd(1).gif" height="350" width="359"/> 
</div>
<div>
【输入格式】
</div>
<div>
输入由若干行组成，第一行有3个整数，$n（1≤n≤100）、m（1≤m≤n^2）,p$；$n$表示村庄数，$m$表示村庄间道路数。第$2$至$m+1$行是每条路的信息，每行三个整数，为道路的起点、终点和两村庄间距离。（村庄从0开始编号）
</div>
<div>
【输出格式】
</div>
<div>
P个整数，学校所在村庄编号(如果P个以上村庄都适合建立学校，选择编号小的P个村庄建学校，输出时按编号从小到大输出)。
</div>
<div>
【输入样例】
</div>
<div>
输入文件名：djsc.in
</div>
<div>
6 8 2<br/>
0 2 10<br/>
0 4 30<br/>
0 5 100<br/>
1 2 5<br/>
2 3 50<br/>
3 5 10<br/>
4 3 20<br/>
4 5 60
</div>
<div>
【输出样例】
</div>
<div>
输出文件名：<span>djsc.out</span> 
</div>
<div>
0 3
</div>
<p>
 
</p>
