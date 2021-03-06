# 题目描述


<h3>
【题目描述】
</h3>
<p>
    韩信是中国军事思想“谋战”派代表人物，被后人奉为“兵仙”、“战神”。“王侯将相”韩信一人全任。“国士无双”、“功高无二，略不世出”是楚汉之时人们对其的评价。作为统帅，他率军出陈仓、定三秦、擒魏、破代、灭赵、降燕、伐齐，直至垓下全歼楚军，无一败绩，天下莫敢与之相争。
</p>
<p>
    相传，韩信带兵打仗时，从不直接清点军队人数。有一次，韩信带 $1500$ 名兵士打仗，战死四五百人。站 $3$ 人一排，多出 $2$ 人；站 $5$ 人一排，多出 $4$ 人；站 $7$ 人一排，多出 $6$ 人。韩信马上说出人数：$1049$。
</p>
<p>
    这次，刘邦派韩信带兵 $N$ 人攻打一座重兵驻扎的城市。城市占领了，可汉军也是伤亡惨重。韩信需要知道汉军<strong>至少</strong>损失了多少兵力，好向刘邦汇报。
</p>
<p>
    已知韩信发出了 $M$ 次命令，对于第i次命令，他选择一个素数 $P_i$，要求士兵每 $P_i$ 人站一排，此时最后一排剩下了 $a_i$ 人。你的任务是帮助韩信求出这种情况下汉军损失兵力的最小值。当然，由于士兵们都很疲惫，他们有可能站错队伍导致韩信得到的数据有误。
</p>
<h3>
【输入格式】
</h3>
<p>
第一行两个正整数 $N,M$，分别代表最初的军队人数和韩信的询问次数。
</p>
<p>
接下来有 $M$ 行，每行两个非负整数 $P_i,a_i$，代表韩信选择的素数和此时剩下的人数。
</p>
<p>
输入保证每个素数各不相同。
</p>
<h3>
【输出格式】
</h3>
<p>
输出一行，一个整数。
</p>
<p>
若有解，输出最小损失人数。若无解，输出 $-1$.
</p>
<h3>
【样例输入】
</h3>
<pre>1500 3
3 2
5 4
7 6
</pre>
<h3>
【样例输出】
</h3>
<pre>31
</pre>
<h3>
【数据范围】
</h3>
<p>
对于 30% 的数据，$1 \leq N \leq 1,000,000$，$1\leq M \leq 4$；
</p>
<p>
对于 50% 的数据，$1 \leq N \leq 100,000,000$，$1 \leq M \leq 8$；
</p>
<p>
对于 100% 的数据，$1 \leq N \leq 1,000,000,000,000$，$1 \leq M \leq 10$；
</p>
<p>
保证所有素数的乘积 $\prod_{i=1}^nP_i\le 10^{12}$，$0 \le a_i &lt; P_i$。
</p>
<br/>
