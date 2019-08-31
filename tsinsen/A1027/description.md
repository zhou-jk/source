<div id="pcont1" style="margin-top:20px; display:block;">

# 问题描述

<div class="pdcont">　　微软的Word有一个拼写检查功能，如果你拼写错了单词，它会用红线标出以示提醒，然后给出可能正确的单词。现在要你编程实现类似的一个系统：给定一个词表以及一个待检查的单词，判断这个单词是否在词表中，如果不在词表中，程序应该给出一个相似的单词。<br/>
　　在寻找相似的单词时，你只需要考虑如下几个简单的情况：<br/>
　　1、漏写了一个字母，如把abacus误拼写为abacs<br/>
　　2、多写了一个字母，如把abacus误拼写为abaacus<br/>
　　3、将某处的一个字母写成了另一个字母，如abacus误拼写为abacup<br/>
　　编程实现这个系统。</div>
# 输入格式

<div class="pdcont">　　输入数据的第一行是一个由小写字母组成的字符串，表示要进行拼写检查的单词<br/>
　　第二行是一个数N（1&lt;=N&lt;=100）,表示词表中词的数目<br/>
　　接下来有N行，每行都是一个由小写字母组成的字符串，代表词表中的每一个单词<br/>
　　所有字符串的长度在2到20之间</div>
# 输出格式

<div class="pdcont">　　仅输出一个字符串：<br/>
　　1、如果要检查的单词在词表中出现，则原样输出该单词<br/>
　　2、如果要检查的单词在词表中未出现，但在词表中找到相似的单词，则输出在词表中和它相似的那个单词。如果在此表中找到多个相似单词，仅输出在输入文件中最靠前的一个。<br/>
　　3、如果要检查的单词在词表中未出现，并且在词表中找不到与它相似的单词，输出NOANSWER</div>
# 样例输入

<div class="pddata">abstaine<br/>
4<br/>
abacus<br/>
abstract<br/>
abstain<br/>
abstainer</div>
# 样例输出

<div class="pddata">abstain</div>

</div>