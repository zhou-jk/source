# 题目描述


<div>
	<p>
		【题目描述】
	</p>
	<p>
		后勤补给对与一个处于战争状态的军团是极其重要的。你作为军团掠夺联队的一员，你的指挥管命令你们去切断敌对军团的后勤补给线路。要想切断敌人的一条交通通道至少需要装载量为w的掠夺小队（假设小队的每个成员的装载量为1）去驻守那里。只要敌人缺少任何一座补给站都将无法进行补给。掠夺联队的兵力并不足以遍布整个宇宙，因此你的指挥官要求你求出如何以最少的兵力切断敌人的后勤补给线路。
	</p>
	<p>
		<br/>
	</p>
	<p>
		【输入格式】
	</p>
	<p>
		第一行为两个整数N、M (2 ≤ N ≤ 500, 0 ≤ M ≤ N × (N − 1) ⁄ 2)  表示有N个安全点，和M条交通通道
	</p>
	<p>
		第i+1至第i+m行，每行三个整数si,ti,wi（0&lt;=s,t<n< span="">, s≠ t,w&gt;0 ）表示s到t有一条交通通道，且货物运输量为wi</n<>
	</p>
	<p>
		<br/>
	</p>
	<p>
		【输出格式】
	</p>
	<p>
		一个整数X表示至少需要多少个军团成员去切断敌人的补给线路
	</p>
	<p>
		如果补给线路本身就不需要兵力输出0<br/>
<br/>
【样例输入】
	</p>
	<p>
		t2bb.in
	</p>
	<p>
		3 3
	</p>
	<p>
		0 1 1
	</p>
	<p>
		1 2 1
	</p>
	<p>
		2 0 1
	</p>
	<p>
		【样例输出】
	</p>
	<p>
		t2bb.out
	</p>
	<p>
		2
	</p>
	<p>
		<br/>
	</p>
</div>
