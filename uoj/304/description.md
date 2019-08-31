# 题目描述

<p>Koala 发明了一个新游戏，来邀请你一起玩！游戏的开始，她会在桌上放 $N$ 个物品，物品从 $0$ 到 $N - 1$ 标号。接着，她会秘密地给每个物品分配一个 $1$ 到 $N$ 之间的整数权值，且任意两个物品不会被分配到相同的权值。其中，第 $i$ 个物品的权值为 $P_i$。她请你来确定由这些权值构成的序列 $P=P_0,P_1,\dots ,P_{N-1}$ 的一些特征。</p>
<p>为了回答她的问题，你可以请 Koala 玩若干轮游戏。每一轮中，你会得到 $W$ 个蓝色石子，Koala 会得到 $W$ 个红色石子。首先，你可以选择若干个物品，再把你的一些（或全部）石子放在这些物品的旁边。Koala 会观察你的石子分配，然后类似地把她的一些（或全部）石子放在若干个物品旁边。如果一个物品旁边的红色石子数严格大于蓝色石子数，那么，Koala可以获得这个物品。Koala 分配她的石子时，总会选择使她获得的物品的权值和最大的方案，如果有多种方案可以做到这一点，她会选择一种获得的物品数最多的方案，如果仍然有多种方案，她会选择其中任意一种。</p>
<p>Koala 非常懒，如果你和她玩太多轮游戏，她就会睡着。你的任务是通过尽可能少轮数的游戏，确定 Koala 的序列 $P$ 的相关特征。</p>
<h2>任务</h2>
<p>在这个任务中，你需要实现 $4$ 个函数：<code>minValue</code>, <code>maxValue</code>, <code>greaterValue</code> 和 <code>allValues</code>。</p>
<p>每个函数需要你确定序列 $P$ 的不同特征。我们强烈推荐在我们提供的模版的基础上进行作答。注意，即使你只想获得部分子任务的分数，你也必须为四个函数都提供一个实现（尽管一些函数的内部可能为空）。你的程序禁止从标准输入读数据、向标准输出写数据或与任何文件交互。</p>
<p>在每个函数中，参数 N 表示游戏中物品的个数，参数 W 表示你和Koala在每一轮游戏中拥有的石子数。</p>
<ul><li><code>minValue(N, W)</code> --- 这个函数需要返回权值最小的物品的标号 $i$，即 $P_i=1$</li>
<li><code>maxValue(N, W)</code> --- 这个函数需要返回权值最大的物品的标号 $i$，即 $P_i=N$</li>
<li><code>greaterValue(N, W)</code> --- 这个函数需要比较物品 $0$ 和物品 $1$ 的权值，返回权值较大的物品的标号。具体来说，若 $P_0&gt;P_1$​，它应该返回 $0$ ，否则返回 $1$ 。</li>
<li><code>allValues(N, W, P)</code> --- 这个函数需要确定整个排列，并将其存放在给定的数组 $P$ 中：具体来说，$P[i]$ 应该保存物品 $i$ 的权值 $P_i (0 \leq i \leq N-1)$。</li>
</ul><p>在每个测试点中，交互库会一次或多次调用这些函数中的一个。每次函数调用代表不同的任务，哪个函数会被调用、以及最多被调用多少次取决于子任务（见下文）。你可以认为 Koala 在每次函数调用前确定了她的序列 $P$，并且序列不会在一次函数的调用过程中改变。一次调用结束后，她可以在下次函数调用之前改变她的序列。</p>
<p>你实现的四个函数可以通过调用函数 <code>playRound</code> 来获取 Koala 的序列的相关信息。</p>
<ul><li><code>playRound(B, R)</code>，请 Koala 和你玩一轮游戏。</li>
</ul><p>数组 B 描述你在每个物品旁边放了多少蓝色石子。具体来说，对任意 $0 \leq i \leq N-1$，$B[i]$ 个蓝色石子将会被放在物品 $i$ 旁边。每个 $B[i]$ 必须是一个非负整数，且 $B[0]+B[1]+\cdots +B[N-1]$ 不能超过 $W$ 。</p>
<p>交互库会把 Koala 的回应存放在你提供的数组 R 中。具体来说，对任意 $0 \leq i \leq N-1$，Koala 会在物品 $i$ 旁边放 $R[i]$ 个红色石子。</p>
<p>每个子任务对你在每次游戏中调用 <code>playRound</code> 的次数有所限制。注意，调用次数越少你的得分可能会越高。（具体限制和评分方式参见下文）</p>
<h4>样例数据：$0$ 分</h4>
<ul><li>有 $5$ 个「样例数据」测试点，每个测试点恰好调用一次 $4$ 个函数中的某一个。请看下文的__样例__获取各测试点的详细信息。</li>
<li>$N=6$</li>
<li>$P=5,3,2,1,6,4$</li>
</ul><p>每次游戏中，你可以调用 <code>playRound</code>至多 $3200$ 次。</p>
<h4>子任务 1：$4$ 分</h4>
<ul><li>在这个子任务中，交互库只会调用函数 <code>minValue</code>，每个测试点中，这个函数最多会被调用 $100$ 次。</li>
<li>$N=100$</li>
<li>$W=100$</li>
<li>每一次游戏中，你可以调用 <code>playRound</code> 至多 $2$ 次。</li>
</ul><h4>子任务 2：$15$ 分</h4>
<ul><li>在这个子任务中，交互库只会调用函数 <code>maxValue</code>。每个测试点中，这个函数最多会被调用 $100$ 次。</li>
<li>$N=100$</li>
<li>$W=100$</li>
<li>每一次游戏中，你可以调用 <code>playRound</code> 至多 $13$ 次。</li>
<li>这个子任务中，一个测试点的分数取决于每一轮游戏中 <code>playRound</code> 被调用次数的最大值 $C_{max}$，具体来说，你的得分为：<ul><li>若 $C_{max}\leq 4$，获得 $15$ 分。</li>
<li>若 $5 \leq C_{max} \leq 13$，获得 $7$ 分。</li>
</ul></li>
</ul><h4>子任务 3：$18$ 分</h4>
<ul><li>在这个子任务中，交互库只会调用函数 <code>greaterValue</code>。每个测试点中，这个函数最多会被调用 $1100$ 次。</li>
<li>$N=100$</li>
<li>$W=100$</li>
<li>每一次游戏中，你可以调用 <code>playRound</code> 至多 $14$ 次。</li>
<li>这个子任务中，一个测试点的分数取决于每一轮游戏中 <code>playRound</code> 被调用次数的最大值 $C_{max}$，具体来说，你的得分为：<ul><li>若 $C_{max}\leq 3$，获得 $18$ 分。</li>
<li>若 $C_{max}=4$，获得 $14$ 分。</li>
<li>若 $C_{max}=5$，获得 $11$ 分。</li>
<li>若 $6 \leq C_{max}\leq 14$，获得 $5$ 分。</li>
</ul></li>
</ul><h4>子任务 4：$10$ 分</h4>
<ul><li>在这个子任务中，交互库只会调用函数 <code>allValues</code>，每个测试点中，这个函数最多会被调用恰好一次。</li>
<li>$N=100$</li>
<li>$W=200$</li>
<li>你可以调用 <code>playRound</code> 至多 $700$ 次。</li>
</ul><h4>子任务 5：$53$ 分</h4>
<ul><li>在这个子任务中，交互库只会调用函数 <code>allValues</code>，每个测试点中，这个函数会被调用恰好一次。</li>
<li>$N=100$</li>
<li>$W=100$</li>
<li>你可以调用 <code>playRound</code> 至多 $3200$ 次。</li>
<li>这个子任务中，一个测试点的分数取决于 <code>playRound</code> 被调用的次数 $C$ ，具体来说，你的得分为：<ul><li>若 $C \leq 100$，获得 $53$ 分。</li>
<li>若 $101 \leq C \leq 3200$，获得 $\lfloor 53-8 \log_2 (c/100) \rfloor$ 分。其中，$\lfloor x \rfloor$ 为不大于 $x$ 的最大整数。举例来说，若 $C=3200$，那么你的解答将获得 $13$ 分。</li>
</ul></li>
</ul><p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<p>本题不支持 hack。</p>