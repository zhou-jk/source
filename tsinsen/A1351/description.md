<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　给定一个长为 n 的序列,序列的每个元素都是一个区间,你需要找到一个尽量长的连续子序列, 使得这个序列的任意两个元素(也是区间)的交均不为空。<br/>
<br/>
　　注意,区间 [1, 1] 不是空,因为这个区间包含一个数 1 。</div>
# 输入格式

<div class="pdcont">　　第一行一个整数 n ,表示序列的长度。<br/>
<br/>
　　接下来 n 行,每行 2 个正整数 L, R ,依次表示一个区间 [L, R] 。如果有多个区间满足要求,请输 出最靠前的。</div>
# 输出格式

<div class="pdcont">　　输出一行两个数 s, t ,表示你找到的子序列为 [s, t] 。如果存在多组最长的子序列,请输出最靠前<br/>
<br/>
　　的一个。</div>
# 样例输入

<div class="pddata">5<br/>
1 5<br/>
2 4<br/>
3 4<br/>
2 2<br/>
2 3</div>
# 样例输出

<div class="pddata">1 3</div>
# 数据规模和约定

<div class="pdcont">　　对于 30% 的数据:n ≤ 100<br/>
　　对于 60% 的数据:n ≤ 1000<br/>
　　对于 80% 的数据:n ≤ 100000<br/>
　　对于 100% 的数据:n ≤ 500000 ,输入的区间均为 [1, 10^8] 的子区间且不为空。</div>

</div>