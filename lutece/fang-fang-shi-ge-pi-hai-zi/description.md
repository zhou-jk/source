
# Content

方方是一个调皮的孩子，每天到处搞破坏把妹子，邻居都讨厌他。一天方方不小心把邻居老姚神的魔法棒给摔成了$n$段，长度分别为$a\_0,a\_1,\cdots,a\_{n-1}$。方方虽然调皮，但还是不敢招惹可怕的老姚神，修复魔棒是如此的艰难，只能请求另一个邻居哈利波特大用魔法把魔棒修复，但哈利波特大正在忙着统计霍格沃茨的男女比例，没有太多时间帮方方修魔棒，只答应只为方方使用一次魔法。

哈利波特大的魔法很奇怪，魔法只能把一段连续的魔棒片段连在一起，并且连接的片段的长度之和必须为$p$的倍数，（例如$n=6$，$p=11$，$a\_0$到$a\_{n-1}$分别为$11,11,1,6,7,9$,哈利波特大可以把$a\_0$和$a\_1$连在一起，或者把$a\_3, a\_4, a\_5$连在一起），注意老姚神的魔棒必须按顺序接，也就是说，方方不能随意改动$a\_0, a\_1,\cdots a\_{n-1}$的顺序。

方方想把尽可能多的魔法棒片段连在一起，现在想找你帮忙。

# Standard Input

第一行包含一个正数 $T$ ($T\leq 50$)，表示数据组数。

接下来每组数据包含两行。

第一行包含两个整数 $n, p$ ($1\leq n\leq 100000, 1\leq p\leq 11$)，代表魔法棒有$n$段，连接的长度之和必须为$p$的倍数。

第二行包含$n$个正整数分别表示$a\_0,a\_1,\cdots ,a\_{n-1}$,($1\leq a\_i\leq 1000, 0\leq i < n$)。

# Standard Output

对于每组数据输出一行，表示能最多能连接起来的魔棒片段个数。

# Samples

<style>
        table,table tr th, table tr td { border:1px solid #0094ff; }
        table { width: 200px; min-height: 25px; line-height: 25px; text-align: center; border-collapse: collapse;}   
    </style>
<table>
	<tr>
		<td>Input</td>
		<td>Output</td>
	</tr>
<tr><td>5
6 11
11 11 1 6 7 9
1 2
1
1 3
3
10 2
1 2 3 4 5 6 7 8 9 10
4 3
1 2 3 4</td><td>3
1
1
9
3</td></tr></table>


# Constraints



# Note

注意在第二组样例中，事实上魔法根本无法施展，但是答案是$1$，因为即使不使用魔法，片段也是一个一个的~

# Source


