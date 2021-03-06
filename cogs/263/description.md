# 题目描述


<p>
 一些矩形的海报、照片或其他同样形状的图片被张贴在墙上。它们的边都是垂直或水平的。每个矩形可以部分或全部覆盖其它矩形。所有矩形组成的集合的边界称为周界。
</p>
<p>
<strong>[ 任务描述 ] ： </strong> 
</p>
<p>
    写一个程序计算周界。
</p>
<p>
下图是一个有 7 个矩形的例子。
</p>
<p>
<strong><img src="/upload/image/20120925/20120925164109_97246.jpg" alt=""/></strong> 
</p>
<p>
        Figure 1. 一个 7 个矩形的集合
</p>
<p>
对应的周界为如图 2 所示所有线段的集合。
</p>
<p>
<img src="/upload/image/20120925/20120925164114_20873.jpg" alt=""/> 
</p>
<p>
        Figure 2. 矩形集合的周界
</p>
<p>
    所有的矩形的坐标都是整数。
</p>
<p>
<strong>[ 输入数据 ] ： </strong> 
</p>
<p>
    文件 PICTURE.IN 的第一行张贴在墙壁上的矩形图片的数目。在随后的行中，每行有两个点的坐标，分别为某一个矩形的左下角和右上角的坐标。每一个坐标由 X 坐标与 Y 坐标组成。
</p>
<p>
样例输入：
</p>
<p>
7 <br/>
-15 0 5 10 <br/>
-5 8 20 25 <br/>
15 -4 24 14 <br/>
0 -6 16 4 <br/>
2 15 10 22 <br/>
30 10 36 20 <br/>
34 0 40 16
</p>
<p>
对应着图 1 的例子。
</p>
<p>
<strong>[ 输出数据 ] ： </strong> 
</p>
<p>
    文件 PICTURE.OUT 包含一行，为一个非负整数，表示输入数据中所有矩形集的周界。
</p>
<p>
样例输出：
</p>
<p>
228
</p>
<p>
<strong>[ 限制 ] ： </strong> 
</p>
<p>
0 &lt;= 矩形数 &lt; 5000
</p>
<p>
所有坐标在 [-10000,10000] 内，结果的值可能需要 32 位有带符号表示。
</p>
