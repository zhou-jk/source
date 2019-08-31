<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　Wayne喜欢排队……不对，是Wayne所在学校的校长喜欢看大家排队，尤其是在操场上站方阵。<br/>
　　某日课间操时，校长童心大发想了一个极具观赏性的列队方案，如下：<br/>
　　1. 方阵排成N行，每行恰好M个学生。<br/>
　　2. 由于校长喜欢女孩子，所以在一行上不能有连续P个男生。<br/>
　　3. 由于校长喜欢女孩子，所以在校长看来，一列全是男生是不好的，全男生的列数不能超过Q。<br/>
　　Wayne因为感冒了所以不用参加列队，不过他看着大家排队排得不亦乐乎，于是他想知道，在男女生数目无限制的情况下，有多少种列队方案？<br/>
　　两种方案被视作不同，表明存在至少一个二元组(i,j)而两种方案中第i行第j列的同学性别不同。另外，因为答案可能很大，所以请把答案模10^9 + 7。</div>
# 输入格式

<div class="pdcont">　　输入仅一行4个正整数，依次是N,M,P,Q。</div>
# 输出格式

<div class="pdcont">　　输出仅一行，表示答案。</div>
# 样例输入

<div class="pddata">2 3 3 1</div>
# 样例输出

<div class="pddata">46</div>
# 数据规模和约定

<div class="pdcont">　　对于5%的数据，满足P = 1。<br/>
　　对于另外10%的数据，满足N * M &lt;= 20。<br/>
　　对于另外15%的数据，满足N &lt;= 2，M &lt;= 10^6。<br/>
　　对于另外10%的数据，满足N &lt;= 2。<br/>
　　对于另外20%的数据，满足N &lt;= 4，P &lt;= 2，Q &lt;= 2。<br/>
　　对于100%的数据，满足1 &lt;= N &lt;= 8，1 &lt;= M &lt;= 10^18，1 &lt;= P &lt;= 3，0 &lt;= Q &lt;= 3。</div>

</div>