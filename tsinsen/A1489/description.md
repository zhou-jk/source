<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　N位同学参与抽奖，每位同学在抽奖箱中放入了若干个写有自己姓名的小球。<br/>
　　抽奖总共有M轮，每轮开始时，从抽奖箱中随机地抽出一个小球，公布上面的姓名，并做记录。之后，将这个小球放回抽奖箱。因此，同一个球被抽出多次是有可能的。<br/>
　　每位同学的名字被抽出的次数越多，他获得的奖金越高。如果写有他的名字的球被抽出了X次，则他将获得奖金X^2元。<br/>
　　为了防止奖金总额超出预算，请你计算出需要支付的总奖金的期望值。另一方面，为了确保尽量多的人能够得奖，请你算出获得奖金大于0的人数的期望值。</div>
# 输入格式

<div class="pdcont">　　第一行包含两个数N和M，代表参加抽奖活动的同学个数，以及抽奖的轮数。<br/>
　　第二行包含N个正整数A1~AN，分别代表N个同学在抽奖箱中放入的小球个数。</div>
# 输出格式

<div class="pdcont">　　输出包含两行，每行包含一个实数，保留两位小数。第一行的实数表示总奖金的期望值，第二行的实数表示获得奖金大于0的人数的期望值。</div>
# 样例输入

<div class="pddata">2 2<br/>
1 1</div>
# 样例输出

<div class="pddata">3.00<br/>
1.50</div>
# 数据规模和约定

<div class="pdcont">　　30%的数据满足N,M≤1000且A1=A2=...=AN=1；<br/>
　　100%的数据满足1≤N,M≤10^5，A1,A2,...,AN≥1且A1+A2+...+AN≤10^9。</div>

</div>