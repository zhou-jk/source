# 

 
 # 题目背景 
此题为taophee专辑中的第四题。 

 
 # 题目描述 
终于进入了森林，Taophee觉得该歇会了，于是便决定，召唤出身为飞侠的YH到附近找些食物。YH不愧为飞侠，很快就找到了一排果子。YH为了尽快回到Taophee身边，所以YH决定使用她的特殊技能——魔法跳跃技能，在最短的时间内收集到果子。<BR>YH观察这一排果子，发现在果子中还有一些荆棘。在这一排树中，如果是果子，则树上有若干个果子(用正数表示)；如果是荆棘，则会造成一些HP伤害(用负数表示)。YH回两种跳跃技能，一种为魔法跳跃，一种为普通跳跃。由于YH魔法有限，YH只能恰好且必须经过n次魔法跳跃和m次普通跳跃后从第一棵树到达最后一棵树，每次跳跃的距离不限，但必须向右跳。每次魔法跳跃所跳过的树，包括终点但不包括起点，如果是果子，YH就摘光树上所有的果子，装入她的背包里；但如果是荆棘，那么YH的HP将会相应的减少。每次普通跳跃，那些树只是被跳过去，不会有任何影响。到达最后一棵树后，YH会从背包里拿出一些果子来补充自己损失的HP，每个果子补充1点HP，直到背包里没有果子或YH的HP补满为止。<BR>Taophee希望尽量得到更多的果子，如果得不到果子，他就希望YH损失的HP能少一些，现在问YH怎样跳才能摘到最多的过子或损失最少的HP？ 

 
 # 输入格式 
输入文件第一行有三个正整数n,m,L(0&lt;=n,m&lt;=50,1&lt;=L&lt;=200,n+m&lt;=L)，n为魔法跳的次数，m为普通跳的次数，L为树的棵数。接下来一行包含L个整数，每个数都在-200到200之间。如果为正数则表示这是果子，数值表示果子的个数；如果为负数则表示这是一个荆棘，数值表示造成的HP伤害。 

 
 # 输出格式 
仅有一行,包含一个整数，表示最多摘到的果子数或最少HP损失数。若为最少HP损失数，则用负数表示。 
# 样例数据
<style>
        table,table tr th, table tr td { border:1px solid #0094ff; }
        table { width: 200px; min-height: 25px; line-height: 25px; text-align: center; border-collapse: collapse;}   
    </style>
<table>
	<tr>
		<td>输入样例</td>
		<td>输出样例</td>
	</tr>
<tr><td>5 5 12
23 23 –12 –27 –2 14 –23 –13 16 –17 –3 27
</td><td>78
</td></tr></table>
