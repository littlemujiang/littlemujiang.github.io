---
layout:     post
title:      "《算法4》勘误表"
subtitle:   " \" 5年前的小成果 \""
date:       2019-01-11 10:00:00
author:     "mujiang"
header-img: "img/post-pages.jpg"
catalog: false
tags:
     - 技术

---

> “赠人玫瑰，手有余香。”


## 前言

2013年刚买此书时，网页版的勘误表看着太麻烦，手工粘50多页又太多，所以就写了个爬虫抓下来了。

现共享之~希望能对大家有所帮助！

PS：
这篇文档的路途也是异常坎坷： 之前放在微盘，后来过期，有网友留言想要，就买了一个月会员下载下来，转存到百度云，最近百度云过期，又有网友想要，就干脆想放到GitHub io上，发现原来的是word文档，便又写了脚本把它转成markdown的table格式。这才有了此文。

时间过去很久，或许新的印次是否已经修复这些错误，或许发现了新的错误，故仅供参考。

<p id = "build"></p>
---

## 正文


#### 《算法4》勘误表


<table style="TABLE-LAYOUT: auto">
<tr> <td>页码</td>  <td>勘误内容</td> <td>印次</td>
<tr> <td>--</td>  <td>扉页 谢路云 ---> 谢路云 译</td> <td>2</td>
<tr> <td>--</td>  <td>译者序 倒数7 瑕不掩玉 ---> 瑕不掩瑜</td> <td>2</td>
<tr> <td>0</td>  <td>彩插第一页，表1.2.14，典型的用例： *Visual*Accumulator a = new *Visual*Accumulator(*T, 10*); 上面的 10 要改为 1.0 。</td> <td>3</td>
<tr> <td>1</td>  <td>彩插，图 4.4.6，右上角那幅图：v  --->  w 的有向边的颜色应该从黑色改为红色。</td> <td>3</td>
<tr> <td>1</td>  <td>第一页中的代码，Public应该是public</td> <td>2</td>
<tr> <td>1</td>  <td>彩插，图 4.3.6：第4幅图和第5幅图中的黑色细线（各1条）均应改为红色细线。</td> <td>3</td>
<tr> <td>1</td>  <td>图 4.4.25 的标题： Bellman-Ford 算法的轨迹  应改为：  Bellman-Ford 算法的轨迹（含负权重环的图）</td> <td>3</td>
<tr> <td>4</td>  <td>1.1.1节，“五种语法”改为“七种语法”</td> <td>3</td>
<tr> <td>5</td>  <td>灰底格式图上面的说明文字“whitelist.txt“作为参数传递给main()  上面的“whitelist.txt”应改为“largeW.txt”。  编辑说明  原书错误</td> <td>3</td>
<tr> <td>6</td>  <td>6页 5行 浮点型 ---> 双精度实数类型，原文没有出现float point字样，7页对double型的注解是双精度实数,float型的注解是单精度实数,应该统一</td> <td>2</td>
<tr> <td>6</td>  <td>正文倒数第7行，算数    改为  算术</td> <td>3</td>
<tr> <td>7</td>  <td>第七页的表 1.1.2 中 double 类型的第二列运算符与第三列典型表达式不相匹配，第一个运算符是 +，而对应的表达式是减法。 3.141 - 0.03  --->  3.141 + 0.03 3.111  --->  3.171  编辑说明  原书问题，不过编辑的时候没看仔细。</td> <td>2</td>
<tr> <td>7</td>  <td>7页 倒数9 32位二进制 ---> 32个二进制位的机器字  编辑说明  字长32位的机器字</td> <td>2</td>
<tr> <td>9</td>  <td>9页 倒数11 i++;。和i--;的意思相同 ---> i++和i--的意思分别与上述的++i和--i相同  编辑说明  i++;和i--;的意思分别与上述的++i;和--i;相同</td> <td>2</td>
<tr> <td>15</td>  <td>代码下面第3行： 原文“可以使用数学模型的来估计程序的性能”，删除“的”</td> <td>3</td>
<tr> <td>16</td>  <td>16页  倒数17 java.utils.Arrays --->  java.util.Arrays</td> <td>2</td>
<tr> <td>16</td>  <td>1.1.7节上面的倒数第7行，“StdIn”应改为“In”。</td> <td>3</td>
<tr> <td>16</td>  <td>1.1.6.8，第5段2行，An Introduction to programming in Java  “Programming” 首字母大写。</td> <td>3</td>
<tr> <td>17</td>  <td>第3行，因为Math.sin()首字母M未用等宽字体。</td> <td>3</td>
<tr> <td>18</td>  <td>表1.1.8： static void initialize(long seed)  初始化  应改为：  static void setSeed(long seed)  设置随机数生成器的种子  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>18</td>  <td>倒数第14行： StdRandom 的 initialize() 方法为随机数生成器提供种子 这里的“initialize”应改为“setSeed”。</td> <td>3</td>
<tr> <td>23</td>  <td>23页，第六行，第一个printf后面的左右括号不是同一个字体，，ps:这算勘误么。。。</td> <td>2</td>
<tr> <td>24</td>  <td>24页，1.1.9.5下面，第六行，StdOt  => StdOut</td> <td>2</td>
<tr> <td>25</td>  <td>我们会使用 In 库中的 readInts()、readDoubles() 和 readStrings() 以及 Out 库中的 writeInts()、writeDoubles() 和 writeStrings() 方法，参数可以是文件或网页如表 1.1.17 所示。   应改为：   我们会使用 In 库中的 readInts()、readDoubles() 和 readStrings() 以及 Out 库中的重载的多个 write() 方法，name 参数可以是文件或网页，如表 1.1.17 所示。  编辑说明  这个是错误的吗，也可以这样说吧？ 当然是错误。因为在表 1.1.17 中，只有三个重载的 write() 方法，没有 writeInts()、writeDoubles() 和 writeStrings() 方法。也就是说，这三个方法的名称都是 write，只不过这三个同名的 write() 方法的第一个参数不同而已。这是非常明显的错误。英文版中就已经错了。</td> <td>3</td>
<tr> <td>25</td>  <td>表 1.1.17，public class Out 下面的第一行： static void write(int[], String name)       应改为：  static void write(int[] a, String name)</td> <td>3</td>
<tr> <td>31</td>  <td>31页 21行 除零 ---> 除以零</td> <td>2</td>
<tr> <td>35</td>  <td>Page 35, 1.1.27 binomial(100,50) => binomial(100,50,.25); booksite上有题目描述，http://algs4.cs.princeton.edu/11model/，没有第三个参数的话，怎么调用题目中的函数呢？</td> <td>2</td>
<tr> <td>35</td>  <td>提高题1.1.27： if (N == 0 && k == 0) return 1.0; and if (N < 0 || k < 0) return 0.0; return (1.0 - p)*binomial(N-1, k, p) + p*binomial(N-1, k - 1);  应改为：  if (N == 0 && k == 0) return 1.0; if (N < 0 || k < 0) return 0.0; return (1.0 - p)*binomial(N-1, k, p) + p*binomial(N-1, k - 1, p); 注意： 1. 删除 and ，分为两行。 2. 最后的 k - 1); 改为  k - 1, p);</td> <td>3</td>
<tr> <td>40</td>  <td>第4行，“标识份”应改为“标识”。</td> <td>3</td>
<tr> <td>44</td>  <td>java.utils.Array.sort() 应改为  java.util.Arrays.sort()</td> <td>3</td>
<tr> <td>46</td>  <td>本书中使用的部分抽象数据类型： Transaction  换位 应改为 Transaction  交易</td> <td>3</td>
<tr> <td>47</td>  <td>Interval2D 测试用例程序中： Point2D p = new Point(x, y); 应改为 Point2D p = new Point2D(x, y);</td> <td>3</td>
<tr> <td>47</td>  <td>47页，程序代码 box = new Interval2D(x,y); =>  box = new Interval2D(xinterval,yinterval);</td> <td>2</td>
<tr> <td>47</td>  <td>第四十七页，Interval2D的测试用例代码，第十一行： Interval2D box = new Interval2D(x, y); 应为： Interval2D box = new Interval2D(xinterval, yinterval);  编辑说明  原书问题。</td> <td>2</td>
<tr> <td>48</td>  <td>表1.2.6倒数第2行 int compareTo(Date that)   改为   int compareTo(Transaction that)</td> <td>3</td>
<tr> <td>50</td>  <td>50页，右边第二段代码，第二行，indexOF => indexOf</td> <td>2</td>
<tr> <td>53</td>  <td>1.2.3.3 实例方法小节 返回值类型和所有参数变量的名称  应改为：  所有参数变量的类型和名称</td> <td>3</td>
<tr> <td>53</td>  <td>1.2.3.3 实例方法： 在一个实例方法中对变量的引用指的是该方法的变量中的值。  应改为：  在一个实例方法中对变量的引用指的是调用该方法的对象中的值。</td> <td>3</td>
<tr> <td>54</td>  <td>第五十四页，1.2.3.4 作用域标题正文第七行，参数方法  --->  参数变量。</td> <td>2</td>
<tr> <td>54</td>  <td>第6行 在静态方法中前两者的用法没有变化   应改为：   前两者的用法和静态方法中一样</td> <td>3</td>
<tr> <td>59</td>  <td>表 1.2.14，典型的用例： *Visual*Accumulator a = new *Visual*Accumulator(T,1.0); 而 T 和 1.0 要加粗。并且 T,1.0 的逗号后面要加一个空格。</td> <td>3</td>
<tr> <td>63</td>  <td>1.2.5.5 节第4行：重写  --->  覆盖</td> <td>2</td>
<tr> <td>65</td>  <td>最后一行： 而且不存在能够引用初始化变量b的那个Date对象的引用了。 这句话中的 b 应改为 a 。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>66</td>  <td>第一行： 唯一引用就是变量b，但是该引用被赋值语句覆盖 这里的 b 应改为 a 。</td> <td>3</td>
<tr> <td>71</td>  <td>练习1.2.5： 答："hello World"。  应改为：  答："Hello World"。</td> <td>3</td>
<tr> <td>72</td>  <td>Page 72,提高题，1.2.15 int[] ints = new int[words.length; => int[] ints = new int[words.length];  编辑说明  原书错误。</td> <td>2</td>
<tr> <td>72</td>  <td>提高题1.2.15： String input = StdIn.readAll(); 改为： String input = in.readAll();  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>74</td>  <td>表1.3.1 泛型可迭代的基础集合数据类型API，先进先出(FIFO)队列： Item dequeue()  删除最近添加的元素  应改为：  Item dequeue()  删除最早添加的元素</td> <td>3</td>
<tr> <td>80</td>  <td>上一页中的 Evaluate 类是该算法的一个实现。  应改为：  本页中的 Evaluate 类是该算法的一个实现。</td> <td>3</td>
<tr> <td>80</td>  <td>代码片段第二处注释  "}" 改为")"</td> <td>3</td>
<tr> <td>84</td>  <td>表1.3.4 void push(Item item)  添加一个字符串 Item pop()         删除最近添加的字符串  应改为：  void push(Item item)  添加一个元素 Item pop()         删除最近添加的元素</td> <td>3</td>
<tr> <td>85</td>  <td>第2段代码： public void push(String item)  应改为：  public void push(Item item)</td> <td>3</td>
<tr> <td>85</td>  <td>第3段代码： public String pop()  应改为：  public Item pop()</td> <td>3</td>
<tr> <td>85</td>  <td>第3段代码： String item = a[--N];  应改为：  Item item = a[--N];</td> <td>3</td>
<tr> <td>87</td>  <td>倒数第6行： 但它无知道数据的表示方法是数组(即实现细节)。  应改为：  但它无需知道数据的表示方法是数组(即实现细节)。</td> <td>3</td>
<tr> <td>88</td>  <td>ResizingArrayQueue 的缺点在于某些 push() 和 pop() 操作会调整数组的大小：这项操作的耗时和栈大小成正比。    这句话中的“ResizingArrayQueue”应改为“ResizingArrayStack”。     编辑说明  勘误带入错误</td> <td>3</td>
<tr> <td>89</td>  <td>倒数3行，first.node 改为 first.next</td> <td>3</td>
<tr> <td>89</td>  <td>倒数2行，它们实现的不是抽象数据类型因为我们会直接使用其实例变量。  改为  抽象数据类型，因为……（缺少逗号）</td> <td>3</td>
<tr> <td>92</td>  <td>92页 19  指向last ---> last用代码字体</td> <td>2</td>
<tr> <td>98</td>  <td>算法1.4 背包：  “算法1.1和算法1.2” 应改为 “算法1.2和算法1.3”。  编辑说明  原书错误</td> <td>3</td>
<tr> <td>100</td>  <td>倒数第8行：运行算法  应改为： 编译算法 。</td> <td>3</td>
<tr> <td>101</td>  <td>第7行：ConcurrentModifi-cationException  应改为： ConcurrentModificationException 。</td> <td>3</td>
<tr> <td>107</td>  <td>提高题1.3.49： 用三个栈实现一个队列，保证每个队列操作(在最坏情况下)都只需要常数次的栈操作。 这里的“用三个栈”应改为“用有限个栈”。</td> <td>3</td>
<tr> <td>110</td>  <td>表1.4.1，典型用例：   StdOut.println(cnt + "triples" + time + "seconds");   应改为：    StdOut.println(cnt + " triples " + time + " seconds"</td> <td>3</td>
<tr> <td>116</td>  <td>3.1节中详细完整地给出了1.1节中所讨论过的命题B的证明 改为 3.1节中的命题B详细完整地给出了1.1节讨论的内容</td> <td>3</td>
<tr> <td>116</td>  <td>中文116页 表1.4.5 向下取整（floor）、向上取整（ceiling）印成了相同的记号   编辑说明  向上取整，符号倒过来。</td> <td>2</td>
<tr> <td>126</td>  <td>倒数第12行： 同一时间最多能在内存中保存 3200 万个 int 值或是 1600 万个 double 值。 上面的“3200 万个”应改为“2.56亿万个”，“1600 万个”应改为“1.28亿万个”。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>128</td>  <td>倒数第3行 “图1.4.9”应改为“图1.4.10”</td> <td>3</td>
<tr> <td>129</td>  <td>图1.4.10 一个 String 对象和一个子字符串： 子字符串举例：   该图右下角的“36字节”应改为“56字节”，计算如下：  1. 对象开销 16 字节。   2. 存放数组长度 4 字节。(数组长度的值是 16 )  3. 存放 16 个 char ("CGCCTGGCGTCTGTAC") 共 32 个字节。(每个 char 占用 2 个字节)  4. 填充字节 4 字节。   编辑说明  原书错误</td> <td>3</td>
<tr> <td>130</td>  <td>倒数第13行：“initialize”应改为“setSeed”。</td> <td>3</td>
<tr> <td>136</td>  <td>1.5.1 小节第4行和第9行：对等关系 应改为 等价关系 。</td> <td>3</td>
<tr> <td>137</td>  <td>第10行：“归并，最终所有的整数属于同一个集合”应改为“归并到同一个集合”。</td> <td>3</td>
<tr> <td>139</td>  <td>倒数第14行：“调用 find() 方法”应改为“调用 connected() 方法”。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>144</td>  <td>第3行：”2i+2“应改为”2i+3“。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>145</td>  <td>算法1.5（续）的代码中： private int find(int p)  应改为：  public int find(int p)  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>155</td>  <td>第16行：“完整的比较序列”  应改为： “全序关系” 。</td> <td>3</td>
<tr> <td>158</td>  <td>第158页，第6行： 对于 0 到 N-1 之间的每一个 i，  应改为：  对于 1 到 N-1 之间的每一个 i，  编辑说明  原书错误</td> <td>3</td>
<tr> <td>161</td>  <td>比较两种排序算法 的程序代码中： // 使用算法1将T个长度为N的数组排序  应改为：  // 使用算法alg将T个长度为N的随机数组排序</td> <td>3</td>
<tr> <td>166</td>  <td>练习 2.1.3： a[j] < a[min])  应改为：  a[j] < a[min] 注意：去掉最右边的右括号。</td> <td>3</td>
<tr> <td>167</td>  <td>提高题 2.1.22： 事务排序测试用例。编写一个 SortTransaction 类，在静态方法 main() 中从标准输入读取一系列事务， 这里的两处“事务”都应改为“交易”。</td> <td>3</td>
<tr> <td>172</td>  <td>第1行 要对子数组 a[10 .. hi] 进行排序，先将它分为 a[10 .. mid] 和 a[mid+1 .. hi] 两部分， 这名话中的两处“10”应改为“lo”。</td> <td>3</td>
<tr> <td>173</td>  <td>命题F 的 证明 中： C(N) ≤ C(┕ N/2 ┘) + C(┌ N/2 ┐) + N  应改为：  C(N) ≤ C(┌ N/2 ┐) + C(┕ N/2 ┘) + N 注：这个公式后面接着说：右边的第一项是将数组的左半部分排序所用的比较次数，第二项是将数组的右半部分排序所用的比较次数，第三项是归并所用的比较次数。</td> <td>3</td>
<tr> <td>173</td>  <td>命题F 的 证明 中：   C(N) ≥ C(┕ N/2 ┘) + C(┌ N/2 ┐) +  ┕N/2 ┘   应改为：    C(N) ≥ C(┌ N/2 ┐) + C(┕ N/2 ┘) +  ┕N/2 ┘ 注意：第一项和第二项调换位置。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>176</td>  <td>命题H的证明： 处理一个数组的遍数正好是 └lgN┘ （即 2^n ≤ N ＜ 2^(n+1)）  应改为：  处理一个数组的遍数正好是 ┌lgN┐  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>187</td>  <td>187页 7行 计算机科学届 ---> 计算机科学界</td> <td>2</td>
<tr> <td>195</td>  <td>表格最后一行： MaxPQ(int max)   创建一个最大容量为 max 的优先队列 这句话中的“最大”应改为“初始”。</td> <td>3</td>
<tr> <td>197</td>  <td>第8行： 从命令行输入一个整数M以及一系列字符串，每一行表示一个事务。  应改为：  从命令行获得一个整数，从输入流获得一系列字符串，输入流的每一行表示一个交易。</td> <td>3</td>
<tr> <td>197</td>  <td>格式中的说明文字最后两句： 所有事务输入完毕之后程序会从优先队列中按递减顺序打印出最大的M个事务。这段代码相当于将所有事务放入一个栈，遍历栈以颠倒它们的顺序并按照增序将它们打印出来。   应改为：   处理完所有交易，优先队列中存放着以增序排列的最大的M个交易。然后这段代码将它们放入到一个栈中，遍历这个栈以颠倒它们的顺序，从而将它们按降序打印出来。</td> <td>3</td>
<tr> <td>198</td>  <td>表2.4.4  A E L M P A E E L M A E E L M  应改为：  A E L M P P A E E L M P P A E E L M P  编辑说明  原书错误</td> <td>3</td>
<tr> <td>201</td>  <td>图2.4.5 堆的操作： 左下角的图中，结点“P”和结点“N”应该对调。 右下角的图中，结点“I”和“H”之间的边应该加上阴影背景，如同结点“S”、“P”和“I”之间的边一样，并且“下沉”的箭头应指向结点“H”，而不是结点“I”。  编辑说明  读者勘误说明：注意，英文版本身就有错误，译者已经改正了一些错误，但还遗漏了一些错误没有改正。 另外，“删除最大元素”的第一幅图最好改为和“插入元素”的修改后的最后一幅图(即左下角的图)一致。但这样跟着的两幅图也要相应修改。</td> <td>3</td>
<tr> <td>202</td>  <td>算法2.6 基于堆的优先队列 的代码中： pq[N+1] = null;   // 防止越界 上面的“越界”应改为“对象游离”。</td> <td>3</td>
<tr> <td>206</td>  <td>命题R 的证明的最后一行： 120次交换(两倍于比较)  应改为：  120次交换(以及两倍的比较)</td> <td>3</td>
<tr> <td>207</td>  <td>图2.4.7 的右上角：连接节点 L 和 节点 E 的边也应该有阴影背景，如同连接节点 M 和节点 L 的边一样。  编辑说明  原书勘误。</td> <td>3</td>
<tr> <td>212</td>  <td>第212页，提高题2.4.34的解答： public void delete(int k) {   exch(k, N--);   swim(qp[k]);   sink(qp[k]);   keys[pq[N+1]] = null;   qp[pq[N+1]] = -1; }  应改为：  public void delete(int k) {   int index = qp[k];   exch(index, N--);   swim(index);   sink(index);   keys[k] = null;   qp[k] = -1; }</td> <td>3</td>
<tr> <td>215</td>  <td>2.5.1.4 廉价的交换 第二行： 因为比较只需要访问元素的一小部分，而排序过程中大部分元素都不会被访问到。 这句话中的“大部分元素”应改为“元素的大部分”。</td> <td>3</td>
<tr> <td>225</td>  <td>提高题2.5.18： 并在调用 sort() 之后再根据保存的索引恢复键的原始顺序。  应改为：  并在调用 sort() 之后再恢复原始的键。</td> <td>3</td>
<tr> <td>226</td>  <td>实验题2.5.32： S.Ioyd  应改为：  S. Loyd</td> <td>3</td>
<tr> <td>228</td>  <td>228页表3.1.2 表体第2行 Value, val  --->  Value val(前一个是参数类型，后一个是参数名)</td> <td>2</td>
<tr> <td>229</td>  <td>表3.1.3 默认实现：  boolean contains(key)     return get(key) != null;   应改为：    boolean contains(Key key)     return get(key) != null;  编辑说明  原书错误，boolean contains(Key key) 在 contains 方法中，Key 是参数的类型，key 是参数的名称。</td> <td>3</td>
<tr> <td>230</td>  <td>3.1.1.7 迭代 小节中第1行和第4行的 Interable<key> 均应改为 Iterable<Key></td> <td>3</td>
<tr> <td>230</td>  <td>230页 表3.1.4 表体第2行 Value, val  --->  Value val  编辑说明  排版出错</td> <td>2</td>
<tr> <td>234</td>  <td>表3.1.7：“TinyTale.txt”应改为“tinyTale.txt”。 勘误说明：第一个字母“T”应改为小写“t”。本书的示例都是在 Linux 操作系统中运行的，而在 Linux 操作系统中，文件名是区分大小写的。</td> <td>3</td>
<tr> <td>235</td>  <td>正文第7行： 例如，用 FrequencyCounter 分析 leipzig1M.txt 中长度不小于 8 的单词意味着，在一个含有数以千计的键值对的符号表中进行上百万次的查找，而互联网中的一台服务器可能需要在含有上百万个键值对的表中处理上亿的交易。 这里的“数以千计”应改为“数十万”。</td> <td>3</td>
<tr> <td>236</td>  <td>图 3.1.2：“红色为新加入的结点”应改为“加粗显示的为新加入的结点”。</td> <td>3</td>
<tr> <td>239</td>  <td>表3.1.8，右边，倒数第3行： 8 4 6 5 11 9 10 3 0 7 上面的 9 应该从灰色改为黑色。</td> <td>3</td>
<tr> <td>241</td>  <td>第241页，算法3.2(续1)，底部： 7  6  6    A C E H L M P R S X ￣￣  应改为：  6  6  6    A C E H L M P R S X 7  6 ￣￣</td> <td>3</td>
<tr> <td>242</td>  <td>算法3.2(续2)，Keys(Key lo, Key hi) 方法中： for (int i = rank(lo); i < rank(hi); i++) q.enqueue(keys[i]);  应改为：  for (int i = rank(lo); i < rank(hi); i++)     q.enqueue(keys[i]); 注：第二行代码应缩格。</td> <td>3</td>
<tr> <td>245</td>  <td>倒数第2行： key[]和val[]  应改为：  keys[]和vals[]</td> <td>3</td>
<tr> <td>245</td>  <td>表3.1.11，右下角（注意断行）：   需要计算每种类型的数据的散列无  法进行有序性相关的操作链接和空  结点需要额外的空间   应改为：    需要计算每种类型的数据的散列  无法进行有序性相关的操作  链接和空结点需要额外的空间</td> <td>3</td>
<tr> <td>246</td>  <td>第2行： key[]  应改为： keys[]（共两处）</td> <td>3</td>
<tr> <td>246</td>  <td>练习3.1.7： Frequency Counter  应改为：  FrequencyCounter</td> <td>3</td>
<tr> <td>247</td>  <td>提高题3.1.23： [N/2] 应改为： ┕N/2┘</td> <td>3</td>
<tr> <td>247</td>  <td>提高题3.1.24 的倒数第2行   ┕ k x - k lo) / (k hi - k lo) ┘   应改为：   ┕ (k x - k lo) / (k hi - k lo) ┘  说明：x、lo、hi 都是下标，勘误为少前括号。</td> <td>3</td>
<tr> <td>248</td>  <td>实验题3.1.37： 在100万个长度为M位的随机整数  应改为：  在100万个长度为M个二进位的随机整数</td> <td>3</td>
<tr> <td>249</td>  <td>实验题3.1.41： 随机的32位整数  应改为：  随机的32二进位(32-bit)整数</td> <td>3</td>
<tr> <td>250</td>  <td>第2自然段第2行： 结点包含的链接可以指向空(null)或者其他结点。  应改为：  结点包含的链接可以为空(null)或者指向其他结点。</td> <td>3</td>
<tr> <td>250</td>  <td>第2自然段第3行： 每个结点只能有一个父结点指向自己  应改为：  每个结点只能有一个父结点</td> <td>3</td>
<tr> <td>254</td>  <td>第4行： (请见练习3.2.12)  应改为：  (请见练习3.2.13)  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>257</td>  <td>倒数第5行： 向上取整函数的计算如图3.2.10所示。 这里的“向上取整”应改为“向下取整”。</td> <td>3</td>
<tr> <td>257</td>  <td>257 页 表3.2.1  第5列 21 1914 55 ---> 21 191 455</td> <td>2</td>
<tr> <td>257</td>  <td>257 页 倒数13行 （floor） --->  floor(key) 同时用代码字体</td> <td>2</td>
<tr> <td>258</td>  <td>258页 第3行 以及≥和≤  --->  以及>和<</td> <td>2</td>
<tr> <td>259</td>  <td>图3.2.11： 在子树中共有8个结点 其中的8改为6，此外，该图中 E 结点上面的 8 也应相应改为 6。</td> <td>3</td>
<tr> <td>260</td>  <td>260页 倒数3 前继 ---> 前趋（predecessor）  编辑说明  前继的翻译也有，但是前趋更好。</td> <td>2</td>
<tr> <td>261</td>  <td>算法3.3(续4) 的说明文字的最后一行： deleteMax() 的实现和 deleteMin() 类似，只需将左改为右即可 这里的“左改为右”应改为“左右互换”。</td> <td>3</td>
<tr> <td>266</td>  <td>提高题3.2.34：ThreadST  应改为  ThreadedST</td> <td>3</td>
<tr> <td>267</td>  <td>提高题3.2.35： limit(2lnN)    应改为   2lnN</td> <td>3</td>
<tr> <td>274</td>  <td>通过对比图3.3.11中的2-3树和表3.2.1中由相同的键构造的二叉查找树你也可以看到，完美平衡的2-3树要平展得多。  应改为：  通过对比图3.3.11中的2-3树和图3.2.8中由相同的键构造的二叉查找树，你也可以看到，完美平衡的2-3树要平展得多。 说明： 1. 表3.2.1 改为 图3.2.8 2. 增加一个逗号。</td> <td>3</td>
<tr> <td>277</td>  <td>第2行： 只需要将 left 换成 right 即可  应改为：  只需将 left 和 right 互换即可</td> <td>3</td>
<tr> <td>277</td>  <td>3.3.2.7标题 向2-结点中插入新键 改为： 向单个2-结点中插入新键</td> <td>3</td>
<tr> <td>279</td>  <td>图3.3.21图题   分解4-结点的同时转换链接的颜色（另见彩插） 改为： 图3.3.21 通过转换链接的颜色来分解4-结点（另见彩插）</td> <td>3</td>
<tr> <td>279</td>  <td>3.3.2.11 小节 第一行“3.3.29”应改为“3.3.2.9”。</td> <td>3</td>
<tr> <td>285</td>  <td>命题H 的 例证 中：  和典型的二叉查找树（例如表3.2.1中所示的树）相比    这里的“表3.2.1”应改为“图3.2.8”。</td> <td>3</td>
<tr> <td>287</td>  <td>287页 表3.3.2标题第3列（N次插入之后） ---> （N次随机插入之后）</td> <td>2</td>
<tr> <td>288</td>  <td>练习3.3.7：   以图3.3.8为例为图中的其他5种情况画出相应的示意图。   应改为：    以图3.3.9为例为图3.3.8中的其他5种情况画出相应的示意图。</td> <td>3</td>
<tr> <td>288</td>  <td>练习3.3.4： log3N 这里的 3 应该是下标。</td> <td>3</td>
<tr> <td>294</td>  <td>与之类似，互联网中使用的 IP 地址也不是随机的，所以如果我们想用除留余数法将其散列就需要用素数(2的幂除外)大小的数组。 这里的“（2的幂除外）”应改为“（特别地，这不是2的幂）”。 说明：英文原文是：(in particular, not a power of 2) 注意，除了素数2以外，其余素数都不是2的幂。 此外，在 Java 等语言中，要计算余数的话，如果除数是2的幂，有很高效的算法。</td> <td>3</td>
<tr> <td>295</td>  <td>3.4.1.6小节第2行： 每种数据类型都需要相应的散列函数，于是 Java 令所有数据类型都继承了一个能够返回一个32位整数的 hashCode() 方法。 这里的“32位整数”应改为“32比特整数”。</td> <td>3</td>
<tr> <td>295</td>  <td>295页 倒数8 2^32中的 ---> 2^32个不同整数中的</td> <td>2</td>
<tr> <td>299</td>  <td>倒数第2行： 从图3.4.4可以看出  应改为：  从图3.4.5可以看出</td> <td>3</td>
<tr> <td>300</td>  <td>3.4.2.3 小节第1-2行： 散列最主要的目的在于均匀地将键散布开来，因此在计算散列后键的顺序信息就丢失了，如图3.4.5所示。 这里的 “，如图3.4.5所示” 应该删除。</td> <td>3</td>
<tr> <td>301</td>  <td>图3.4.6中，第一行标为5的那一列，键C对应的值均应从5改为4(共8处)。对应的彩插也应该修改。</td> <td>3</td>
<tr> <td>301</td>  <td>图 3.4.6：“红色的是新插入的键”应改为“加粗的是新插入的键”。</td> <td>3</td>
<tr> <td>302</td>  <td>第14行的 N++; 应左移一格，和第13行对齐。</td> <td>3</td>
<tr> <td>302</td>  <td>格式中的说明文字： 这段符号表的实现将键和值分别保存在两个数组（BinarySearchST类型）中，使用空（标记为null）来表示一簇键的结束。 这句话中的“数组（BinarySearchST类型）中”应改为“数组中（与BinarySearchST类型中一样）”。</td> <td>3</td>
<tr> <td>304</td>  <td>命题M讨论第6-7行： 键簇的平均长度在两种情况下都是 N/(2N)=1/2，但未命中的查找所需的探测次数在最好情况下为1（所有的查找都至少需要一次探测）加上 (0+1+0+1+...)/(2N)=1/2，在最坏情况下为 1+(N+(N-1)+...)/(2N)～N/4。 上面的“所需的探测次数”应改为“所需的平均探测次数”，“1+(N+(N-1)+...)/(2N)～N/4”中的第一个+改为“加上”</td> <td>3</td>
<tr> <td>309</td>  <td>第2行："将K长度加倍"应改为“将长度加倍”。</td> <td>3</td>
<tr> <td>310</td>  <td>提高题3.4.25： “修改3.4.19节” 应改为 “修改3.4.1.8节”。</td> <td>3</td>
<tr> <td>312</td>  <td>最后一段 大多数程序员的第一选择都是散列表，在其他因素更重要时才会选择红黑树。在第5章我们会遇到这个“第一选择”的例外：当键都是长字符串时，我们可以构造出比红黑树更灵活而又比散列表更高效的数据结构。    应改为：    根据经验法则，大多数程序员的第一选择都是散列表，在其他因素更重要时才会选择红黑树。在第5章我们会遇到这个经验法则的例外：当键都是长字符串时，我们可以构造出比红黑树更灵活而又比散列表更高效的数据结构。  编辑说明  没看出区别啊？ 大有区别。第一选择是散列表，第二选择是红黑树，这两者都是经验法则的选择。按照原来的说法，是说在5章遇到“第一选择”的例外，非常有可能是第二选择。而修改后的说法，是经验法则的例外，是第三种选择。而且英文原文就是这么说的。</td> <td>3</td>
<tr> <td>312</td>  <td>表3.5.1：“48N+64M”应改为“48N+32M”。 勘误说明：请参阅第306页表3.4.2。  编辑说明  原书错误。</td> <td>3</td>
<tr> <td>312</td>  <td>最后一段： 大多数程序员的第一选择都是散列表，在其他因素更重要时才会选择红黑树。在第5章我们会遇到这个“第一选择”的例外：当键都是长字符串时，我们可以构造出比红黑树列灵活而又比散列表列高效的数据结构。  应改为：  根据经验法则，大多数程序员的第一选择都是散列表，在其他因素更重要时才会选择红黑树。在第5章我们会遇到这个经验法则的例外：当键都是长字符串时，我们可以构造出比红黑树列灵活而又比散列表列高效的数据结构。</td> <td>3</td>
<tr> <td>312</td>  <td>312页 表3.5.1标题第3列（N次插入之后） ---> （N次随机插入之后）</td> <td>2</td>
<tr> <td>314</td>  <td>Dedup过滤器代码框： StdOut.println(key);  应改为：  StdOut.print(key + " ");</td> <td>3</td>
<tr> <td>315</td>  <td>白名单边滤器代码框：  StdOut.println(word);   应改为：   StdOut.print(word + " ");</td> <td>3</td>
<tr> <td>315</td>  <td>315页 倒数11 路由器 ---> 因特网/互联网路由器</td> <td>2</td>
<tr> <td>318</td>  <td>格式中的说明文字： 第二行“分隔符由命令行参数指定”，这里的“分隔符”应改为“键和值所在的位置”。</td> <td>3</td>
<tr> <td>320</td>  <td>表3.5.5：“标识语”应改为“标识符”。</td> <td>3</td>
<tr> <td>321</td>  <td>格式代码： if (!st.contains(key)) st.put(key, new Queue<string>()); if (!ts.contains(val)) ts.put(val, new Queue<String>()); 这两个 if 语句均应左移六格，和上一句对齐。 StdOut.println(“ ” + s); 上述在两个 for 循环中两个输出语句中的全角双引号要改为半角双引号。</td> <td>3</td>
<tr> <td>322</td>  <td>格式代码最后一条语句： StdOut.println(“  ” + file.getName()); 这条语句中的全角双引号应改为半角双引号。</td> <td>3</td>
<tr> <td>326</td>  <td>练习3.5.15： 编写一个程序，从标准输入接受一个字符串和一个整数 k 作为参数，在标准输出中有序打印出在字符串中找到的 k 元文法（k-gram），以及每个 k-gram 在字符串中的位置。 这里的“和一个整数 k 作为参数”应改为“并从命令行参数获得一个整数 k”。  编辑说明  勘误说明：字符串是从标准输入获得的，而整数 k 是从命令行参数获得的。</td> <td>3</td>
<tr> <td>326</td>  <td>表3.5.6： 所有不在该集合中的键的集合  应改为：  所有在universe中并且不在该集合中的键的集合</td> <td>3</td>
<tr> <td>327</td>  <td>提高题3.5.22： 以及一个允许使用者指定键和值的列的测试用例。  应改为：  以及一个允许使用者指定每次查询的键和值所在的列的测试用例。</td> <td>3</td>
<tr> <td>327</td>  <td>提高题3.5.26第二行：“最近访问过”应改为“最近最少访问”。</td> <td>3</td>
<tr> <td>327</td>  <td>提高题3.5.20： （请见表3.5.5）  应改为：  （请见第320页“图书索引”段落中“对照索引”的定义）</td> <td>3</td>
<tr> <td>331</td>  <td>倒数第9行：“该连接”应改为“这条边”。</td> <td>3</td>
<tr> <td>333</td>  <td>第2行至第3行： 一般来说，如果一幅图中不同的边的数量只占顶点总数 V 的一小部分，那么我们就认为这幅图是稀疏的，否则则是稠密的，参见图 4.1.6。 这里的“只占顶点总数 V 的一小部分”应改为“在顶点总数 V 的一个小的常数倍以内”。</td> <td>3</td>
<tr> <td>334</td>  <td>表 4.1.2，计算所有顶点的平均度数： public static double avgDegree(Graph G) { return 2 * G.E() / G.V(); } 这里的 2 应改为 2.0 。</td> <td>3</td>
<tr> <td>335</td>  <td>图 4.1.10：“都被标记为红色”应改为“都加粗显示”。 说明：相应的彩插不用修改。</td> <td>3</td>
<tr> <td>336</td>  <td>Graph 数据类型 代码框：  adj[w].add(v);    // 将v添加到W的链表中 应改为 adj[w].add(v);    // 将v添加到w的链表中</td> <td>3</td>
<tr> <td>349</td>  <td>第349页，表 4.1.6 后面第1行到第2行： 它能够从标准输入中读取一幅图并打印其中的连通分量数，其后是每个子图中的所有顶点，每行一个子图。 这里的“从标准输入中”应该删去。</td> <td>3</td>
<tr> <td>350</td>  <td>代码后第1行：DepthfirstSearch 应改为 DepthFirstSearch 。</td> <td>3</td>
<tr> <td>350</td>  <td>倒数第7行：“比 union-find 法快”应改为“比 union-find 算法快”。</td> <td>3</td>
<tr> <td>350</td>  <td>第350页，右上角： % more tyinG.txt  应改为：  % java Graph tinyG.txt</td> <td>3</td>
<tr> <td>351</td>  <td>图 4.1.21 的标题： 使用深度优先搜索的轨迹，寻找所有连通分量  应改为：  使用深度优先搜索寻找所有连通分量的轨迹</td> <td>3</td>
<tr> <td>351</td>  <td>图 4.1.21： | | |  5 完成 | | |  检查 6 | | |  检查 3 | | 4 完成 | 6 完成 | dfs(2)       0       T   *T* T T T T        0   *0* 0 0 0 0 | | 检查 0 | 2 完成 上面 *T* 表示 T 是加粗的。而 *0* 位置的 0 应该加粗（书中没有加粗）。</td> <td>3</td>
<tr> <td>351</td>  <td>图 4.1.21： 0 完成 dfs(7)         1     T T T T T T T       0 0 0 0 0 0 0   1  <== 这个 1 要左移一格，对齐下一行 | dfs(8)        1    T T T T T T T T     0 0 0 0 0 0 0 1  1 | | 检查 7 | 8 完成</td> <td>3</td>
<tr> <td>351</td>  <td>图 4.1.21： | | 检查 7 | 8 完成 7 完成 dfs(9)        2    T T T T T T T T T         0 0 0 0 0 0 0 1 1 2 | dfs(11)     2    T T T T T T T T T T     T      0 0 0 0 0 0 0 1 1 2    2 | | 检查 9 说明：dfs(9) 那一行在最后一个加粗的 T 前面应该增加一个 T 。也就是这一行需要有10个 T，其中最后一个 T  是加粗的。</td> <td>3</td>
<tr> <td>353</td>  <td>第7行：Routes.txt 应改为 routes.txt 。</td> <td>3</td>
<tr> <td>354</td>  <td>图 4.1.23 左边： movie vertex       应改为：  电影名 右边： performer vertex  应改为：  演员</td> <td>3</td>
<tr> <td>355</td>  <td>图 4.1.24，无向图 Graph G，顶点 1 的邻接表： 4 7 3 应改为  4 7 0 。</td> <td>3</td>
<tr> <td>356</td>  <td>符号图的数据类型 代码框，最后一个注释： // 将每一行的顶点和该行的其他顶点相连  应改为：  // 将每一行的第一个顶点和该行的其他顶点相连</td> <td>3</td>
<tr> <td>357</td>  <td>% java DegreesOfSeparation movies.txt "/" "Bacon, Kevin"  Kidman, Nicole     Bacon, Kevin     Few Good Men, A (1992)     Cruise, Tom     Days of Thunder (1990)     Kidman, Nicole  Grant, Cary     Bacon, Kevin     Mystic River (2003)     Willis, Susan     Majestic, The (2001)     Landau, Martin     North by Northwest (1959)     Grant, Cary   应改为：   % java DegreesOfSeparation movies.txt "/" "Bacon, Kevin"  Kidman, Nicole     Bacon, Kevin     Woodsman, The (2004)     Grier, David Alan     Bewitched (2005)     Kidman, Nicole  Grant, Cary     Bacon, Kevin     Planes, Trains & Automobiles (1987)     Martin, Steve (I)     Dead Men Don't Wear Plaid (1982)     Grant, Cary</td> <td>3</td>
<tr> <td>358</td>  <td>间隔的度数 代码框中的说明文字：BreadthFirstPath 应改为 BreadthFirstPaths 。</td> <td>3</td>
<tr> <td>359</td>  <td>答疑： 你也可以将用时增加 lgN 并直接用 ST 而非 Bag 来实现 adj()  应改为：  你也可以将用时变为原来 lgV 倍并直接用 ST 而非 Bag 来实现 adj()</td> <td>3</td>
<tr> <td>360</td>  <td>图 4.1.26：“会显示为红色”应改为“会加粗显示”。</td> <td>3</td>
<tr> <td>360</td>  <td>练习4.1.7： 用命令行参数命名并从输入流中接受一幅图  应改为：  从命令行参数指定名字的输入流中接受一幅图</td> <td>3</td>
<tr> <td>361</td>  <td>练习 4.1.17：GraphProper-ties 应改为 GraphProperties 。</td> <td>3</td>
<tr> <td>361</td>  <td>练习 4.1.17： 含有 s 的最小环为 s 到某个顶点 v 的最短距离加上 v 到 s 的最短距离  应改为：  含有 s 的最小环为 s 到某个顶点 v 的最短路径加上从 v 返回到 s 的边 说明：最小环是一些边的集合，而不是距离。这里的某个顶点 v 必须位于 s 的邻接表中，从而存在从 v 返回到 s 边。</td> <td>3</td>
<tr> <td>361</td>  <td>练习 4.1.22： 将值为无穷大的人归为一类(不与 Kevin Bacon 连通)。  应改为：  将值为无穷大的人(不与 Kevin Bacon 连通)归为一类。</td> <td>3</td>
<tr> <td>361</td>  <td>练习 4.1.25： 输出类似如右侧框注所示的数据格式  应改为：  输出类似右侧框注所示的数据</td> <td>3</td>
<tr> <td>362</td>  <td>第362页，提高题 4.1.34： 如果一个顶点被删掉后图不再连通  应改为：  如果一个顶点（以及和它相连的边）被删掉后图不再连通</td> <td>3</td>
<tr> <td>362</td>  <td>提高题 4.1.36：EulideanGraph 应改为 EuclideanGraph 。</td> <td>3</td>
<tr> <td>362</td>  <td>实验题 4.1.41：EulideanGraph 应改为 EuclideanGraph 。</td> <td>3</td>
<tr> <td>362</td>  <td>实验题 4.1.41：RandomEulideanGraph 应改为 RandomEuclideanGraph 。</td> <td>3</td>
<tr> <td>362</td>  <td>实验题 4.1.42：EulideanGraph 应改为 EuclideanGraph 。</td> <td>3</td>
<tr> <td>363</td>  <td>实验题 4.1.43： 从这些顶点构成的子图中随机选取 V 个顶点  应改为：  从这幅图中随机选取 V 个顶点</td> <td>3</td>
<tr> <td>363</td>  <td>实验题 4.1.45：EulideanGraph 应改为 EuclideanGraph 。</td> <td>3</td>
<tr> <td>364</td>  <td>倒数第2行：“和无环图一样”应改为“和无向图一样”。</td> <td>3</td>
<tr> <td>364</td>  <td>倒数第1行：一般性的有向图 应改为 一般性的有向路径 。</td> <td>3</td>
<tr> <td>364</td>  <td>倒数第1行：当存在从 v 到 w 的路径时 应改为 当存在从 v 到 w 的有向路径时 。</td> <td>3</td>
<tr> <td>367</td>  <td>第5行：单点可达性 这五个字应使用黑体，后面加一个句号。</td> <td>3</td>
<tr> <td>367</td>  <td>表 4.2.3 后面第2行：多点可达性 这五个黑体的字后面应加一个句号。</td> <td>3</td>
<tr> <td>367</td>  <td>命题 D 后面第1行：有向样图 应改为 示例有向图 。</td> <td>3</td>
<tr> <td>368</td>  <td>倒数第4行：单点有向路径 应改为 单点有向路径。（黑体）</td> <td>3</td>
<tr> <td>368</td>  <td>第368页，倒数第2行：单点最短有向路径  这八个字应使用黑体，后面加一个句号。</td> <td>3</td>
<tr> <td>369</td>  <td>图 4.2.3： | | | | | | dfs(3)5 | | | | 检查 | | | |  应改为：  | | | | | | dfs(3) | | | | 检查 5 | | | |</td> <td>3</td>
<tr> <td>370</td>  <td>第370页，图 4.2.4：这幅图中有 5 个对象被误标记为潜在的可访问对象，实际上它们是可被回收的对象。这 5 个对象是：左下角的 3 个对象，中部靠右的 2 个对象。 解决方案是： 1. 增加一条 最下边的 可以被直接访问的对象 指向 左下角被误标记为潜在的可访问对象 的 有向边 。 2. 改变 中部靠右的 2 个被误标记为潜在可访问对象 中 左边一个的对象 指向左方的有向边 的方向 。</td> <td>3</td>
<tr> <td>371</td>  <td>图 4.2.8： Calculs、Linear Algebra、Introduction to CS、Advanced Programming、Algorithms、Theoretical CS、Artificial Intelligence、Robotics、Machine Learning、Neural Networks、Databases、Scientific Computing、Computational Biology  应改为：  微积分、线性代数、计算机科学导引、高级编程、算法、计算机科学理论、人工智能、计算机机器人、机器学习、神经网络、数据库、科学计算、计算生物学</td> <td>3</td>
<tr> <td>371</td>  <td>第371页，倒数第5行：定义。有向无环图（DAG）就是一幅不含有环的有向图。 应改为 有向无环图（DAG）就是一幅不含有向环的有向图。</td> <td>3</td>
<tr> <td>371</td>  <td>倒数第4行：因此，解决有向图检测的问题可以回答下面这个问题 这里的“有向图检测”应改为“有向环检测”。</td> <td>3</td>
<tr> <td>371</td>  <td>倒数第2行：边 v→w  应改为： 有向边 v→w 。</td> <td>3</td>
<tr> <td>372</td>  <td>第1行： 请见后面框注“寻找有向环”中的 DirectedCycle 基于这个思想实现了表 4.2.5 中的 API 。 这句话有语法错误，改为 请见后面框注“寻找有向环”，该框注中的 DirectedCycle 基于这个思想实现了表 4.2.5 中的 API 。</td> <td>3</td>
<tr> <td>373</td>  <td>4.2.4.3 小节第1行：优先级限制下的调度问题等价于计算有向无环图中的所有顶点的拓扑排序 这里的“拓扑排序”应改为“拓扑顺序”。</td> <td>3</td>
<tr> <td>373</td>  <td>第373页，倒数第3行：有序无环样图  应改为： 示例有向无环图 。</td> <td>3</td>
<tr> <td>374</td>  <td>图 4.2.10：1 完成        4 5 1        *1*5 4 上面的 *1* 表示加粗的 1，这个加粗的 1 后面应该改插入一个空格。 4 5 1 的 1 应该加粗。</td> <td>3</td>
<tr> <td>374</td>  <td>图 4.2.10：    3  完成          4 5 1 12 11 10 9 6 0 3       3 0 6 9 10 11 12 1 5 4  2 完成  检查 3            4 5 1 12 11 10 9 6 0 3 2     2 3 0 6 9 10 11 12 1 5 4   应改为：     3 完成          4 5 1 12 11 10 9 6 0 3       3 0 6 9 10 11 12 1 5 4  2 完成            4 5 1 12 11 10 9 6 0 3 2     2 3 0 6 9 10 11 12 1 5 4  检查 3   编辑说明  原书有误</td> <td>3</td>
<tr> <td>374</td>  <td>图 4.2.10：  dfs(0)    0    dfs(5)       0   5      dfs(4)     0  5  4                 队列       队列       栈  4完成        4        4    5完成              4   5           54    dfs(1)        0  5  4  1   应改为：  dfs(0)         0    dfs(5)       0  5      dfs(4)     0  5  4              队列       队列        栈  4 完成            4          4    5 完成              4   5           5 4    dfs(1)        0  5  4  1   编辑说明   说明： 1. 第1行的 0 左移半格，对齐下行。 2. 第2行的 5 左移半格，对齐下行。 3. 第4行中间的 4 左移半格，对齐下行。 4. 第5行的最后一个 4 之前插入1个空格。</td> <td>3</td>
<tr> <td>375</td>  <td>命题 4.5 拓扑排序  应改为： 算法 4.5 拓扑排序 。</td> <td>3</td>
<tr> <td>376</td>  <td>第1段代码后第1行：这段代码使用了 DepthFirstOrder 类和 DirectedCycle 类来返回一幅有向无环图的拓扑排序。 这里的“拓扑排序”应改为“拓扑顺序”。</td> <td>3</td>
<tr> <td>376</td>  <td>第1段代码后的第4行：因为它和 SymbolGraph（请见表 4.1.1）的代码几乎相同 这里的：（请见表 4.1.1） 应改为： （请见第 356 页）。</td> <td>3</td>
<tr> <td>376</td>  <td>页面底部： Calculus/Linear Algebra Artificial Intelligence/Neural Networks/Robotics/Machine Learning Machine Learning/Neural Networks  应改为：  Calculus/Linear Algebra Artificial Intelligence/Neural Networks/Robotics/Machine Learning Machine Learning/Neural Networks 说明：应该删除一行空行。</td> <td>3</td>
<tr> <td>376</td>  <td>命题 F。一幅有向无环图的拓扑排序即为所有顶点的逆后序排列 改为 一幅有向无环图的拓扑顺序即为所有顶点的逆后序排列</td> <td>3</td>
<tr> <td>377</td>  <td>命题 G 的证明：第二遍深度优先搜索产生了顶点的逆后序排序 这里的“排序”应改为“排列”。</td> <td>3</td>
<tr> <td>377</td>  <td>第377页，倒数第1行：然后在计算新的调度安排 改为 然后再计算新的调度安排</td> <td>3</td>
<tr> <td>377</td>  <td>第377页： % java Topological jobs.txt "/" Calculus Linear Algebra Introduction to CS Advanced Programming Algorithms Theoretical CS Artificial Intelligence Robotics Machine Learning Neural Networks Databases Scientific Computing Computational Biology  应改为：  % java Topological jobs.txt "/" Calculus Linear Algebra Introduction to CS Advanced Programming Algorithms Theoretical CS Artificial Intelligence Robotics Machine Learning Neural Networks Databases Scientific Computing Computational Biology 说明：应该删除两个空行。</td> <td>3</td>
<tr> <td>378</td>  <td>4.2.5.1 小节第2行和第7行：平等关系 应改为 等价关系。</td> <td>3</td>
<tr> <td>378</td>  <td>4.2.5.1 小节第7行和第8行： 平等的部分 应改为 等价类 每个部分 应改为 每个等价类</td> <td>3</td>
<tr> <td>380</td>  <td>算法 4.6： % java KosarajuSCC tinyDG.txt 5 components 1 0 5 4 3 2 11 12 9 10 6 8 7  应改为：  % java KosarajuSCC tinyDG.txt 5 components 1 5 4 3 2 0 12 11 10 9 6 8 7</td> <td>3</td>
<tr> <td>380</td>  <td>图 4.2.15，中间一列（灰色的字）： v done  应改为：  v 完成 s done  应改为：  s 完成</td> <td>3</td>
<tr> <td>381</td>  <td>命题 H 的证明，倒数第 7 行： 证明的核心在于，按照后逆序进行的深度优先搜索意味着 应改为 证明的核心在于，按照逆后序进行的深度优先搜索意味着</td> <td>3</td>
<tr> <td>381</td>  <td>倒数第2行：dfs(b) 应改为 dfs(6) 。</td> <td>3</td>
<tr> <td>381</td>  <td>倒数第3行：（标记顶点 5、4、3 和 2）  应改为： （标记顶点 0、5、4、3 和 2） 。</td> <td>3</td>
<tr> <td>381</td>  <td>第8行：图 4.2.4 应改为 图 4.2.15 。</td> <td>3</td>
<tr> <td>381</td>  <td>倒数第7行到倒数第6行： 图 4.2.16 所示为 Kosaraju 算法处理 tinyDG.txt 时的轨迹。在每次 dfs() 调用轨迹的右侧都是有向图的一部分，顶点按搜索结束的顺序排列。 应改为 图 4.2.16 所示为 Kosaraju 算法处理 tinyDG.txt 时的轨迹。在每次 dfs() 调用轨迹的右侧都是有向图的一种画法，顶点按搜索结束的顺序排列。。</td> <td>3</td>
<tr> <td>383</td>  <td>第1行：kosaraju 算法  应改为：  Kosaraju 算法 （首字母大写）。</td> <td>3</td>
<tr> <td>384</td>  <td>第10行到第11行：但两条不可能都存在  应改为： 但不可能两条都存在。</td> <td>3</td>
<tr> <td>384</td>  <td>倒数第12行到倒数第11行： 样图只有 13 条边，但它的传递闭包含有可能的 169 条边中的 102 条。  应改为：  示例有向图只有 22 条有向边，但它的传递闭包含有可能的 169 条有向边中的 102 条。 说明： 13 改为 22 样图 改为 示例有向图 边 改为 有向边 （两处）</td> <td>3</td>
<tr> <td>384</td>  <td>图 4.2.18：  5 | T T T T T T  上面第 6 个 T 是灰色的，第 5 个 T 应加粗。 相应的彩插中，第 5 个 T 应从黑色改为红色。  编辑说明  原书错</td> <td>3</td>
<tr> <td>385</td>  <td>最后1个自然段第2行：无环图  应改为： 无向图 。</td> <td>3</td>
<tr> <td>385</td>  <td>最后1个自然段第3行到第4行： 我们将在 4.4 节中遇到加权有向图，这些算法将是学习更加复杂的算法的基础。  应改为：  这些算法是 4.4 节中更复杂的算法的基础，在 4.4 节中我们将学习加权有向图。</td> <td>3</td>
<tr> <td>385</td>  <td>表 4.2.10： 4.2.4.2 框注“查找有向环”  应改为： 4.2.4.2 框注“寻找有向环”。</td> <td>3</td>
<tr> <td>386</td>  <td>练习 4.2.2：（请见图 4.1.10） 应改为： （请见图 4.1.9）。</td> <td>3</td>
<tr> <td>386</td>  <td>练习 4.2.8：（参考练习 4.1.28） 应改为： （参考练习 4.1.27）。</td> <td>3</td>
<tr> <td>387</td>  <td>练习 4.2.17：后逆序  应改为： 逆后序 。</td> <td>3</td>
<tr> <td>387</td>  <td>提高题 4.2.20：欧拉环是一条每条边只出现一次的有向环。 应改为 欧拉环是一条每条边恰好出现一次的有向环。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.26：（将每个强连通分量看作一个顶点） 应改为： （每个强连通分量都是一个顶点）。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.31： 有向欧拉图 应改为 有向欧几里得图 。 4.1.37 应改为 练习 4.1.36 。  EulideanDigraph 应改为 EuclideanDigraph 。</td> <td>3</td>
<tr> <td>388</td>  <td>实验题 4.2.34：练习 4.1.41  应改为：  练习 4.1.40 。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.35： 随机欧拉图  应改为：  随机欧几里得有向图 。 练习 4.1.42  应改为：  练习 4.1.41 。 EulideanDigraph  应改为：  EuclideanDigraph 。 RandomEulideanDigraph  应改为：  RandomEuclideanDigraph 。</td> <td>3</td>
<tr> <td>388</td>  <td>实验题 4.2.36： 练习 4.1.43  应改为：  练习 4.1.42 。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.30： 遍历一遍所有边并使用练习 4.2.7 给出的 Degress 类来初始化数组以及一条含有所有顶点的队列。  应改为：  遍历一遍所有边并使用练习 4.2.7 给出的 Degress 类来初始化该数组以及一个含有所有起点的队列。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.30： 从队列中删去一个顶点并将其标记 应改为 从队列中删去一个起点并将其标记 。</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.30： 如果顶点的入度变为 0，将它插入顶点队列 这里的 顶点队列 应改为 起点队列 。</td> <td>3</td>
<tr> <td>388</td>  <td>实验题 4.2.36：EulideanDigraph  应改为：  EuclideanDigraph 。</td> <td>3</td>
<tr> <td>388</td>  <td>实验题 4.2.37：  从这些顶点构成的子图中随机选取 V 个顶点   应改为：   从这幅有向图中随机选取 V 个顶点</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.37： 然后再从这些顶点构成的子图中随机选取 E 条边来构造一幅图  应改为 然后再从这些顶点构成的子图中随机选取 E 条有向边来构造一幅图 。</td> <td>3</td>
<tr> <td>388</td>  <td>实验题 4.2.38：   从这些顶点构成的子图中随机选取 V 个顶点    应改为：    从这幅有向无环图中随机选取 V 个顶点</td> <td>3</td>
<tr> <td>388</td>  <td>提高题 4.2.38：  然后再从这些顶点构成的子图中随机选取 E 条边来构造一幅图   应改为 然后再从这些顶点构成的子图中随机选取 E 条有向边来构造一幅图</td> <td>3</td>
<tr> <td>390</td>  <td>定义 框：加权无向图 应改为 加权图 。</td> <td>3</td>
<tr> <td>390</td>  <td>最后1行：比如图 4.3.2b  应改为：  比如图 4.3.1 。</td> <td>3</td>
<tr> <td>391</td>  <td>第2行： 而且也完全不一定会和距离成正比。  应改为：  而且也完全不一定会和距离成正比，请见图 4.3.2b。</td> <td>3</td>
<tr> <td>391</td>  <td>图 4.3.2，(c)权重可能是0或者负数：  1 2  0.50  (黑色) 1 3  0.97  (黑色) 2 6  0.17  (灰色)  应改为：  1 2  0.50  (灰色) 1 3  0.97  (黑色) 2 6  0.17  (黑色)</td> <td>3</td>
<tr> <td>391</td>  <td>定义：不重复  应改为： 不重叠 。</td> <td>3</td>
<tr> <td>392</td>  <td>命题 J 的证明：另 e 为权重最小的横切边 应改为 令 e 为权重最小的横切边</td> <td>3</td>
<tr> <td>393</td>  <td>表 4.3.2： 将这条边 e 与 that 比较  应改为：  将这条边与 that 比较</td> <td>3</td>
<tr> <td>394</td>  <td>第8行：无环图  应改为：  无向图 。</td> <td>3</td>
<tr> <td>394</td>  <td>图 4.3.7，最后一行： → 2 7 .34 → 1 7 .19 → 0 7 .16 → 5 7 .28 → 5 7 .28  应改为：  → 2 7 .34 → 1 7 .19 → 0 7 .16 → 5 7 .28 → 4 7 .37</td> <td>3</td>
<tr> <td>395</td>  <td>带权重的边的数据类型 代码框： else throw new RuntimeException(“Inconsistent edge”); ... { return String.format(“%d-%d %.2f”, v, w, weight); }  应改为：  else throw new RuntimeException("Inconsistent edge"); ... { return String.format("%d-%d %.2f", v, w, weight); }  编辑说明  说明：全角的双引号改为半角的双引号。</td> <td>3</td>
<tr> <td>396</td>  <td>4.3.2.2 小节：无环图  应改为： 无向图 。</td> <td>3</td>
<tr> <td>396</td>  <td>4.3.3.3 小节第2行：edge()  应改为： edges() 。</td> <td>3</td>
<tr> <td>396</td>  <td>4.3.3.3 自环 上面的 4.3.3.3  应改为： 4.3.2.3 。</td> <td>3</td>
<tr> <td>397</td>  <td>右下角：... [还有293条边]  应改为： 239 。</td> <td>3</td>
<tr> <td>398</td>  <td>命题 L：任意加权无向图  应改为： 任意加权连通图 。</td> <td>3</td>
<tr> <td>399</td>  <td>第21行到22行： 树中的新顶点旁边有个星号。  应改为：  新加入的边的旁边标有星号。</td> <td>3</td>
<tr> <td>399</td>  <td>图 4.3.10，左上角： * 表示新加入顶点  应改为：  * 表示新加入的边</td> <td>3</td>
<tr> <td>399</td>  <td>图4.3.10，第3幅图旁边的优先队列的最后一行： 0-6  0.58  应改为：  6-0  0.58</td> <td>3</td>
<tr> <td>399</td>  <td>图4.3.10，第3幅图旁边的优先队列的最后一行：   0-6  0.58     应改为：     6-0  0.58   彩插也要相应修改。</td> <td>3</td>
<tr> <td>400</td>  <td>命题 M 的证明：（请见第 2 章的命题 O） 命题 O  应改为： 命题 Q 。</td> <td>3</td>
<tr> <td>401</td>  <td>代码： int v = e.either(), w = e.other(v);         // 跳过失效的边 if (marked[v] && maked[w]) continue;  应改为：  int v = e.either(), w = e.other(v); if (marked[v] && maked[w]) continue;  // 跳过失效的边</td> <td>3</td>
<tr> <td>401</td>  <td>代码 后面说明文字： "一个由顶点索引的队列来标记树的顶点" 应改为 "一个由顶点索引的数组来标记树的顶点"</td> <td>3</td>
<tr> <td>402</td>  <td>第7行：将 v 和树连接  应改为： 将 w 和树连接 。</td> <td>3</td>
<tr> <td>402</td>  <td>倒数第4行： 由 0-6 替换 2-6  应改为：  由 6-0- 替换 6-2</td> <td>3</td>
<tr> <td>402</td>  <td>第1行：“一条边 v”应改为“一个顶点 v”。</td> <td>3</td>
<tr> <td>402</td>  <td>第402页，右边的图的标题： 4.3.12 Prim 算法的轨迹（即时版本，另见彩插）  应改为：  图 4.3.12 Prim 算法的轨迹（即时版本，另见彩插） 说明：加一个“图”字，彩插也相应修改。</td> <td>3</td>
<tr> <td>402</td>  <td>倒数第13行至倒数第10行： 边 4-7 和 2-7 不会影响到优先队列，因为它们的权重分别都大于连接顶点 2 和 4 与最小生成树的最小边。 勘误说明：边 2-7 的确不会影响到优先队列。但是边 4-7 (0.37) 会影响到优先队列，要用它替换右边的图 4.3.12 中的边 0-4 (0.38)，直到边 4-5 (0.35) 替换它为止。总共需要修改图 4.3.12 中的第 2、3、4、5 图的边 4-7 和边 0-4 的颜色以及相应的文字。彩插也需要修改。</td> <td>3</td>
<tr> <td>404</td>  <td>命题N的证明： 因为优先队列中的边数最多为V， 这里的“边数”应改为“顶点数”。</td> <td>3</td>
<tr> <td>404</td>  <td>倒数第2行： 由 0-4 替换为 4-5  应改为：  由 4-7 替换为 4-5</td> <td>3</td>
<tr> <td>404</td>  <td>第2行：IndexPQ  应改为： IndexMinPQ 。</td> <td>3</td>
<tr> <td>404</td>  <td>第404页，命题 N 的证明：（请见第2章命题Q）  应改为： （请见第2章命题Q（续））。</td> <td>3</td>
<tr> <td>404</td>  <td>命题 N 的证明：已知在基于堆实现中的索引优先队列中 ...应该为 已知在基于堆实现的索引优先队列中</td> <td>3</td>
<tr> <td>405</td>  <td>命题 O：任意加权无向图  应改为： 任意加权连通图 。</td> <td>3</td>
<tr> <td>406</td>  <td>第4行：Connected()  应改为： connected()</td> <td>3</td>
<tr> <td>406</td>  <td>算法 4.8 的代码：  MinPQ<Edge> pq = new MinPQ<Edge>(G.edges());   应改为：   MinPQ<Edge> pq = new MinPQ<Edge>();  for (Edge e : G.edges()) pq.insert(e);</td> <td>3</td>
<tr> <td>407</td>  <td>倒数第2行：平行最小生成树算法  应改为： 并行最小生成树算法 。</td> <td>3</td>
<tr> <td>407</td>  <td>练习 4.3.9：EdgeWeighted Graph  应改为：  EdgeWeightedGraph 。  编辑说明  说明：删除一个空格。</td> <td>3</td>
<tr> <td>410</td>  <td>提高题 4.3.30：欧拉加权图  应改为： 欧几里得加权图</td> <td>3</td>
<tr> <td>410</td>  <td>提高题 4.3.30：练习 4.1.37  应改为： 练习 4.1.36  。</td> <td>3</td>
<tr> <td>410</td>  <td>实验题 4.3.34：练习 4.1.41  应改为： 练习 4.1.40 。</td> <td>3</td>
<tr> <td>410</td>  <td>提高题 4.3.33：如果给定的一组边是一棵最小生成树 应该为 如果给定的一组边是一棵生成树</td> <td>3</td>
<tr> <td>410</td>  <td>提高题 4.3.33： 则这最小生成一组边就是图的最小生成树  应改为：  则这组边就是图的最小生成树</td> <td>3</td>
<tr> <td>410</td>  <td>实验题 4.3.34 第2行：随机加权有向图 应改为 随机加权图 。</td> <td>3</td>
<tr> <td>411</td>  <td>实验题 4.3.35：随机欧拉加权图  应改为： 随机欧几里得加权图 。</td> <td>3</td>
<tr> <td>411</td>  <td>实验题 4.3.35：练习 4.1.42  应改为： 练习 4.1.41 。</td> <td>3</td>
<tr> <td>411</td>  <td>实验题 4.3.36：练习 4.1.43  应改为： 练习 4.1.42 。</td> <td>3</td>
<tr> <td>411</td>  <td>实验题 4.3.37： 从这些顶点构成的子图中随机选取 V 个顶点  应改为：  从这幅巨型加权无向图中随机选取 V 个顶点</td> <td>3</td>
<tr> <td>413</td>  <td>第7行：欧拉距离  应改为： 欧几里得距离 。</td> <td>3</td>
<tr> <td>413</td>  <td>图 4.4.2：该图中的第3幅有误，应按照下文中的方法修改： http://www.ituring.com.cn/article/35262</td> <td>3</td>
<tr> <td>414</td>  <td>第8行，加权有向图的数据结构比加权无向图的数据结构更加简单  应改为：  有向边的数据结构比无向边更加简单</td> <td>3</td>
<tr> <td>414</td>  <td>倒数第5行：“加权有向边的数据结构”和“加权有向图的数据结构”  结构 应改为 类型 。</td> <td>3</td>
<tr> <td>414</td>  <td>倒数第3行： WeightedEdge  应改为： DirectedEdge 。</td> <td>3</td>
<tr> <td>415</td>  <td>第415页，倒数第1行：  public Iterable<Edge> adj(int v)   应改为：   public Iterable<DirectedEdge> adj(int v)</td> <td>3</td>
<tr> <td>416</td>  <td>倒数第1行： Iterable<Direc-tedEdge> pathTo(int v)  从顶点 s 到 v 的路径，如果不存在则为 null 这里的 <Direc-tedEdge>  应改为： <DirectedEdge>  。</td> <td>3</td>
<tr> <td>417</td>  <td>第14行至第17行： 在下面的框注中使用了 tinyEWD.txt 文件，它定义了一幅较小的样图中所有的边和权重  应改为：  图 4.4.4 中的 tinyEWD.txt 文件定义了一幅较小的示例有向图中所有的边和权重</td> <td>3</td>
<tr> <td>417</td>  <td>图 4.4.5：  3| 7 ---> 3 0.37 0.97  4| 0 ---> 4 0.38 0.38  5| 4 ---> 5 0.35 0.73  6| 3 ---> 6 0.52 1.49   应改为：   3| 7 ---> 3 0.39 0.99  4| 0 ---> 4 0.38 0.38  5| 4 ---> 5 0.35 0.73  6| 3 ---> 6 0.52 1.51</td> <td>3</td>
<tr> <td>420</td>  <td>命题 P 的证明的最后： 所以以下等式必然成立。 OPT SW <= distTo[w] <= OPT SW  应改为：  所以我们有以下不等式： OPT SW <= distTo[w] <= OPT SW， 且等号必然成立。  编辑说明  说明：上面的 SW 均为下标。</td> <td>3</td>
<tr> <td>422</td>  <td>第6行到第7行： 该路径上的所有顶点均在树中且路径上的最后一条边为 edgeTo[w]  应改为：  该路径上的中间顶点在树中且路径结束于横切边 edgeTo[w]</td> <td>3</td>
<tr> <td>423</td>  <td>第423页，图4.4.10，右边第4组： 3 7 ---> 3 0.37 0.90  应改为：  3 7 ---> 3 0.39 0.99 右边第5、6、7、8组： 3 7 ---> 3 0.37 0.97  应改为：  3 7 ---> 3 0.39 0.99 另外，相应的彩插也需要修改。</td> <td>3</td>
<tr> <td>423</td>  <td>图 4.4.10，右边第 6、7、8 组：  6 3 ---> 6 0.52 1.49  应改为：   6 3 ---> 6 0.52 1.51 另外，相应的彩插也需要修改。 请参见：http://www.ituring.com.cn/article/35510</td> <td>3</td>
<tr> <td>424</td>  <td>任意顶点对之间的最短路径 框注 中的代码：  Iterable<Edge> path(int s, int t)   应改为：   Iterable<DirectedEdge> path(int s, int t)</td> <td>3</td>
<tr> <td>424</td>  <td>第11行：  public Iterable<Edge> pathTo(int v)       //    API中的查询方法）  应改为：   public Iterable<DirectedEdge> pathTo(int v)  //    API中的查询方法）</td> <td>3</td>
<tr> <td>424</td>  <td>代码框 后第1段文字： Dijkstar 算法的实现每次都会为最短路径树添加一条边，该边由一个树中的顶点指向一个非树顶点 w 且它是到 s 最近的顶点。 这段文字应上移至代码框内。</td> <td>3</td>
<tr> <td>424</td>  <td>倒数第10行：欧拉图  应改为： 欧几里得图 。</td> <td>3</td>
<tr> <td>424</td>  <td>倒数第9行：顶点欧拉间距  应改为： 顶点的欧几里得距离 。</td> <td>3</td>
<tr> <td>424</td>  <td>倒数第6行到倒数第5行：欧拉图  应改为： 欧几里得图 。</td> <td>3</td>
<tr> <td>428</td>  <td>代码框中： 5 to 3 (0.62): 5 ---> 1 0.32  1 ---> 3 0.29   应改为：   5 to 3 (0.61): 5 ---> 1 0.32  1 ---> 3 0.29</td> <td>3</td>
<tr> <td>428</td>  <td>第428页，第5行： // 请见4.4.1.5框注“顶点的松驰”  应改为：  // 请见4.4.2.5框注“顶点的松驰”</td> <td>3</td>
<tr> <td>428</td>  <td>第6行到第9行： public double distTo(int v)   // 最短路径树实现中的标准查询算法（请见4.4.1.6  框注“最短路径API的查询方法”） public boolean hasPathTo(int v) public Iterable<Directed Edge> pathTo(int v)  应改为：  public double distTo(int v)  // 最短路径树实现中的标准查询算法 public boolean hasPathTo(int v)    // （请见4.4.2.6框注“最短路径 public Iterable<DirectedEdge> pathTo(int v) // API的查询方法”） 说明：请参见第424页中的同样内容： 1. 4.4.1.6 改为 4.4.2.6 。 2. 删除 Directed Edge 中间的空格。 3. 注释应该针对全部的3行代码，而不是仅针对第1行代码。</td> <td>3</td>
<tr> <td>428</td>  <td>命题 T 的证明第2行：权重变为负值  应改为： 权重取相反数 。</td> <td>3</td>
<tr> <td>428</td>  <td>命题 T 的证明第3行：权重变为正值  应改为： 权重取相反数 。</td> <td>3</td>
<tr> <td>428</td>  <td>public double distTo(int v)   // 最短路径树实现中的标准查询算法（请见4.4.1.6  框注“最短路径API的查询方法”） public boolean hasPathTo(int v) public Iterable<Directed Edge> pathTo(int v)  应改为：  public double distTo(int v)     // 最短路径树实现中的标准 public boolean hasPathTo(int v)            // 查询算法（请见4.4.2.6框注 public Iterable<DirectedEdge> pathTo(int v)   // “最短路径API中的查询方法”） 说明： 这个 // 引导的注释必须分为三行，针对这三个方法，而不是仅针对第一个方法。 Directed Edge 改为 DirectedEdge      (删除中间的空格) 4.4.1.6  改为  4.4.2.6</td> <td>3</td>
<tr> <td>429</td>  <td>将顶点 6 和边 6→2、6→4 和 6→0 添加到树中；  应改为：  将顶点 6 和边 6→2、6→4 和 6→0 添加到树中，边 5→4 已经失效；</td> <td>3</td>
<tr> <td>429</td>  <td>图 4.4.14，第6幅：  刚刚失效 红色箭头往下指的那个，太长了，指到了 边 6 ---> 0。应该缩短点，指到 边 6 ---> 2 就行了。</td> <td>3</td>
<tr> <td>429</td>  <td>4.4.5.2 小节的标题：平行任务调度  应改为： 并行任务调度 。</td> <td>3</td>
<tr> <td>429</td>  <td>倒数第7行到倒数第6行： 给定一组需要完成的特定任务  应改为：  给定一组需要完成的任务和每个任务所需的时间 说明：其中 每个任务所需的时间 所需的时间 用楷体。</td> <td>3</td>
<tr> <td>431</td>  <td>图 4.4.17： 图中的关键路径: s ---> 0 ---> 9 ---> 6 ---> 8 ---> 2 ---> t, 必须加粗显示。</td> <td>3</td>
<tr> <td>433</td>  <td>第1行： 开始如表 4.4.7 所示。  应改为：  开始。前面添加的限制如表 4.4.7 所示。</td> <td>3</td>
<tr> <td>434</td>  <td>图 4.4.18： 为每个任务的结束顶点指出的权重为零的边  应改为：  从每个任务的结束顶点指出的权重为零的边 说明：请参阅第431页图 4.4.16 中的相同内容。</td> <td>3</td>
<tr> <td>435</td>  <td>命题 W 后第1行： 注意，要求最短路径上的任意顶点都不存在负权重环意味着最短路径是简单的  应改为：  注意，要求最短路径上的任意顶点都不存在于负权重环中意味着最短路径是简单的 说明：请参阅 命题 W 中同样的表述。</td> <td>3</td>
<tr> <td>435</td>  <td>倒数第1行： 从本节的开始，我们会不断为最短路径问题加上各种限制并找到解决相应问题的办法。  应改为：  从本节的开始到现在，我们为最短路径问题加上各种限制，使得我们能够找到解决相应问题的算法。 说明：原来的说法：我们会...，表示的是将要做的事情。实际上这是已经做过的事情。后面的句子是： 首先，我们不允许负权重边的存在；其次不接受有向环。现在我们放宽所有这些条件并重点解决一般有向图中的以下问题。</td> <td>3</td>
<tr> <td>437</td>  <td>图 4.4.22，左边从上往下数第2幅的右侧：  3        （灰色）   应改为：   3 1 ---> 3 （灰色）</td> <td>3</td>
<tr> <td>437</td>  <td>倒数第3行：队列 q  应改为： 队列 queue 。</td> <td>3</td>
<tr> <td>437</td>  <td>图 4.4.22，左上角：q  应改为： queue 。</td> <td>3</td>
<tr> <td>437</td>  <td>放松边 4 → 7、4 → 5 并将顶点 7 和 4 加入队列。  应改为：  放松边 4 → 7、4 → 5 并将顶点 7 和 5 加入队列。</td> <td>3</td>
<tr> <td>438</td>  <td>第5行到第6行：4.4.2.4 节框注“边的松驰”  应改为： 4.4.2.5 节框注“顶点的松驰” 。</td> <td>3</td>
<tr> <td>438</td>  <td>命题 Y 的证明：都小于 V-1  应改为： 都不大于 V-1 。</td> <td>3</td>
<tr> <td>439</td>  <td>代码中： public double distTo(int v)       // 最短路径树实现中的标准查询算法（请见4.4.2.6节“最短路                     径API的查询方法”） public boolean hasPathTo(int v)  public Iterable<Edge> pathTo(int v)   // 4.4.6.8节框注”Bellman-Ford“的负权重检测方法  应改为：   public double distTo(int v)           // 最短路径树实现中的标准查询算法  public boolean hasPathTo(int v)          // （请见4.4.2.6框注“最短路径  public Iterable<DirectedEdge> pathTo(int v) // API的查询方法”）   编辑说明  说明：请参见第424页中的同样内容： 1. Edge 改为 DirectedEdge。 2. 注释应该针对全部的3行代码，而不是仅针对第1行代码 3. 删除：// 4.4.6.8节框注”Bellman-Ford“的负权重检测方法</td> <td>3</td>
<tr> <td>439</td>  <td>代码的倒数第2行： // 请见 6.4.6.8 节  应改为：  // 请见 4.4.6.8节框注”Bellman-Ford“算法的负权重检测方法 注意：6.4.6.8 改为 4.4.6.8</td> <td>3</td>
<tr> <td>439</td>  <td>代码中倒数第3行： public Iterable<Edge> negativeCycl()  应改为：  public Iterable<DirectedEdge> negativeCycl()</td> <td>3</td>
<tr> <td>439</td>  <td>代码的说明文字第2行： （以避免出现重复顶点）  应改为：  （队列中不出现重复的顶点） 说明：以避免出现重复顶点是 boolean 数组 onQ[] 的任务。</td> <td>3</td>
<tr> <td>439</td>  <td>倒数第9行：q  应改为： queue 。</td> <td>3</td>
<tr> <td>439</td>  <td>代码第12行：!this.hasNegativeCycle() 改为：!hasNegativeCycle()</td> <td>3</td>
<tr> <td>440</td>  <td>第5行：放松无效的边  应改为： 放松失效的边 。</td> <td>3</td>
<tr> <td>440</td>  <td>表 4.4.8 后面第1行： 实现这些方法并不困难，如以下代码所示。  应改为：  实现这些方法并不困难，如第442页的代码所示。</td> <td>3</td>
<tr> <td>440</td>  <td>倒数第5行：tive-Cycle  应改为： tiveCycle 。</td> <td>3</td>
<tr> <td>442</td>  <td>右上角的代码框中的倒数第2行： public Iterable<Edge> negativeCycl()   应改为：   public Iterable<DirectedEdge> negativeCycl()</td> <td>3</td>
<tr> <td>442</td>  <td>图 4.4.25，最上方：队列  应改为： queue 。  图 4.4.24，最上方：队列  应改为： queue 。</td> <td>3</td>
<tr> <td>442</td>  <td>图 4.4.25：  第4幅图应该删除。 第3幅图需要修改如下：  边 2→7 需要从黑色改为灰色。  edgeTo[4] 的值需要从 0 改为 5，即图中的 4 0 ---> 4 0.07 改为 4 5 ---> 4 0.07 。  edgeTo[7] 的值需要从 2 改为 4，即图中的 7 2 ---> 7 0.44 改为 2 4 ---> 7 0.44 。  编辑说明  请参见：http://www.ituring.com.cn/article/35831</td> <td>3</td>
<tr> <td>444</td>  <td>图 4.4.27： 将每个权重W替换为-Ln(w)  应改为：  将每个权重w替换为-ln(w) 说明： 1. 第一个 W 从大写改为小写 。 2. Ln 改为 ln 。</td> <td>3</td>
<tr> <td>445</td>  <td>倒数第9行：用临接矩阵表示  应改为： 用邻接矩阵表示 。</td> <td>3</td>
<tr> <td>445</td>  <td>倒数第6行：提高到  应改为： 减少到 。</td> <td>3</td>
<tr> <td>445</td>  <td>倒数第5行到倒数第4行： 由于 Bellman-Ford 算法计算普通应用的运行时间常常是线性的，因此在最坏情况下它的运行时间是 VE 。  应改为：  Bellman-Ford 算法计算普通应用的运行时间常常是线性的，在最坏情况下它的运行时间是 VE 。</td> <td>3</td>
<tr> <td>446</td>  <td>第9行：EdgeWe-ightedGraph  应改为： EdgeWeightedGraph 。</td> <td>3</td>
<tr> <td>446</td>  <td>练习 4.4.3：请参考练习 4.3.9  应改为： 请参考练习 4.3.10 。</td> <td>3</td>
<tr> <td>446</td>  <td>练习 4.4.4： 从 tinyEWD.txt 中（请见图 4.4.4）删去顶点 7 并给出加权有向图中以顶点 0 为起点的最短路径树，使用父链接数组表示这棵树。  应改为：  在 tinyEWD.txt 中（请见图 4.4.4）删去顶点 7 。画出加权有向图中以顶点 0 为起点的最短路径树，并使用父链接数组表示这棵树。</td> <td>3</td>
<tr> <td>446</td>  <td>练习 4.4.10： 将练习 4.4.4 中定义的有向图看作无向图，该无向图中的每条边对应有向图中的两条方向不同但权重相同的边。为对应的有向图回答练习 4.4.6 中的问题。  应改为：  将练习 4.4.4 中定义的有向图中的边看作无向边，即每条边对应加权有向图中的两条方向不同但权重相同的边。为对应的加权有向图回答练习 4.4.6 中的问题。</td> <td>3</td>
<tr> <td>448</td>  <td>第448页，提高题 4.4.27：欧拉图  应改为： 欧几里得图 。</td> <td>3</td>
<tr> <td>449</td>  <td>实验题 4.4.48：欧拉图  应改为： 欧几里得图 。</td> <td>3</td>
<tr> <td>452</td>  <td>表5.0.1  Char[] a 改为char[] a</td> <td>3</td>
<tr> <td>452</td>  <td>第452页，第18行到第19行：（为此 Java 提供了一个 StringBuilder 类，请见图 5.0.1）  应改为： （为此 Java 提供了一个 StringBuilder 类）</td> <td>3</td>
<tr> <td>452</td>  <td>第452页，倒数第6行：查找子字符串  应改为： 提取子字符串 。</td> <td>3</td>
<tr> <td>452</td>  <td>正文第7行：lengt()应改为length()</td> <td>3</td>
<tr> <td>453</td>  <td>第453页，正文倒数第3行： 第463页，正文倒数第4行： 第467页，倒数第17行： Alphabet.UNICODE  应改为： Alphabet.UNICODE16 。</td> <td>3</td>
<tr> <td>453</td>  <td>第453页，表 5.0.2： 表示一个索引所需的位数  应改为：  表示一个索引所需的比特数</td> <td>3</td>
<tr> <td>453</td>  <td>页面正中： 方法 R() 和 lgR() 用来获取字母表中的字符数以及表示它们所需的位数 这里的“位数”应改为“比特数”。</td> <td>3</td>
<tr> <td>454</td>  <td>第4行：655 36  应改为： 65 536 。</td> <td>3</td>
<tr> <td>454</td>  <td>第5行到第6行： 它从命令行接受一个字符串并在标准输出上打印输入的每个字符串的出现频率  应改为：  它从命令行接受一个字符串并打印出从标准输入获得的每个字符的出现频率</td> <td>3</td>
<tr> <td>455</td>  <td>第5行到第6行： 第一类方法会从右到左检查键中的字符。这种方法一般被称为低位优先（LSD）的字符串排序。使用数字（digit）代替字符（character）的原因要追溯到相同方法在各种数学类型中的应用。 这里的“低位优先（LSD）”改为“低位优先（least-significant-digit, LSD）”。</td> <td>3</td>
<tr> <td>455</td>  <td>第9行到第10行：高位优先（MSD）建议改为：高位优先（most-significant-digit, MSD）。</td> <td>3</td>
<tr> <td>455</td>  <td>5.1.1 小节第3行到第4行： 同时也是本节中将要学习的两三种字符串排序算法的基础  应改为：  同时也是本节中将要学习的三种字符串排序算法中两种的基础</td> <td>3</td>
<tr> <td>455</td>  <td>第14行： 要学习的第一种方法会将相同字符的键划入同一个切分  应改为：  要学习的第一种方法会为每个字符创建一个切分 说明：这句话的前一句是： 它们的区别之处在于高位优先的字符串排序算法在切分时仅使用键的第一个字符，而快速排序的比较则会涉及键的全部。 因此，这句话中的“字符”是指“键的第一个字符”，“相同字符的键”说不通。也可参见下句话，它说： 第二种方法则总会产生三个切分，分别对应被搜索键的第一个字符小于、等于或大于切分键的第一个字符的情况。</td> <td>3</td>
<tr> <td>459</td>  <td>命题 B 的证明： 由命题 A 可知，该命题完全依赖于键索引计数法的实现是稳定的。  应改为：  该命题完全依赖于键索引计数法的实现是稳定的，这种稳定性已经在命题 A 中指出了。</td> <td>3</td>
<tr> <td>464</td>  <td>倒数第6行：（R = 655 36） 应改为： （R = 65 536）。</td> <td>3</td>
<tr> <td>464</td>  <td>图 5.1.12：字符串的结尾大于任何字符 这里的“大于”应改为“小于”。</td> <td>3</td>
<tr> <td>465</td>  <td>倒数第5行：然而  应改为： 因此 。</td> <td>3</td>
<tr> <td>465</td>  <td>代码框中： { // 对前 d 个字符排序，从a[lo]到a[hi]  应改为：  { // 从第 d 个字符开始对 a[lo] 到 a[hi] 排序</td> <td>3</td>
<tr> <td>466</td>  <td>图 5.1.14，第2栏，倒数第3行：  *s*urely  应改为： *su*rely  。   编辑说明  说明：*s* 表示 s 是黑色的，其余字符是灰色的。</td> <td>3</td>
<tr> <td>466</td>  <td>命题C这特殊格式的文字向前移两段。</td> <td>3</td>
<tr> <td>467</td>  <td>倒数第4行：然后递归适当修正方法  应改为： 然后适当修改递归调用 。</td> <td>3</td>
<tr> <td>467</td>  <td>命题 D：7wN + 3wR  应改为： ～7wN + 3wR 。</td> <td>3</td>
<tr> <td>468</td>  <td>倒数第6行：5.1.2.3 框注  应改为： 5.1.3.3 小节的框注 。 说明： 1. 并不存在 5.1.2.3 小节。 2. 这个框注是“对前 d 个字符均相同的字符串执行插入排序”，见第465页。 3. 这个框注在逻辑上是属于第464页到第465页的“5.1.3.3 小型子数组”小节的，但是在书中印刷在第465页的“5.1.3.5 额外空间”小节中。 4. 虽然这不是严重错误，但是如有可能的话，还是应该把这个框注前移到“5.1.3.3 小型子数组”小节中。 5. 注意，不要前移得太多，因为在“5.1.3.3 小型子数组”中有句话是这么说的： 我们使用了后面框注“对前 d 个字符均相同的字符串执行插入排序”中给出一个版本的插入排序。 必须前移到这句话之后，如果前移太多到了这句话之前就悲剧了。 6. 不知道编辑确认这条勘误时会不会把我的这么多废话删除掉？ :(</td> <td>3</td>
<tr> <td>469</td>  <td>图 5.1.7：这个 图 5.1.7 本身 应改为： 图 5.1.17 。</td> <td>3</td>
<tr> <td>470</td>  <td>5.1.4.4 小节第1行： 且键前面的大半部分首字母均相同  应改为：  且键前面的大半部分字母均相同</td> <td>3</td>
<tr> <td>470</td>  <td>命题 E 的证明：根据命题 D  应改为： 根据命题 C 。</td> <td>3</td>
<tr> <td>470</td>  <td>倒数第5行：web.log.txt  应改为： week.log.txt 。</td> <td>3</td>
<tr> <td>474</td>  <td>第474页，倒数第7行：the sea shore  应改为： the shore 。</td> <td>3</td>
<tr> <td>475</td>  <td>第5行：操作的的实现  应改为： 操作的实现 。</td> <td>3</td>
<tr> <td>476</td>  <td>倒数第3行：字符查找树  应改为： 单词查找树 。</td> <td>3</td>
<tr> <td>477</td>  <td>第1行：关联性数组  应改为： 关联数组 。</td> <td>3</td>
<tr> <td>477</td>  <td>第477页，第3行： 在所有情况下，我们都会检查键中的每个字符并为它们在树中创建一个对应的结点。  应改为：  在所有情况下，对于键中的每个字符，我们或者进行检查，或者在树中创建一个对应的结点。</td> <td>3</td>
<tr> <td>478</td>  <td>图 5.2.4： 这幅图有3处错误。其中表示 l（两处）和 s 的箭头的起始位置应往右移一格。  编辑说明  请参见：http://www.ituring.com.cn/article/36043</td> <td>3</td>
<tr> <td>479</td>  <td>倒数第3行：（请见 5.2.1.8节） 应改为： （请见 5.2.1.10节）。</td> <td>3</td>
<tr> <td>480</td>  <td>第480页，图 5.2.5：  she  by sea sells she  shell   应改为：   she  by sea sells she  shel  shell</td> <td>3</td>
<tr> <td>481</td>  <td>单词查找树中的通配符匹配 代码框：  public void collect(Node x, String pre, String pat, Queue<String> q)  应改为 private void collect(Node x, String pre, String pat, Queue<String> q)</td> <td>3</td>
<tr> <td>482</td>  <td>第4行：在进行  应改为： 再进行 。</td> <td>3</td>
<tr> <td>483</td>  <td>图 5.2.8： 非空链接  应改为：  非空链接，不能删去结点 （返回指向结点的链接）</td> <td>3</td>
<tr> <td>483</td>  <td>第1行： 框注“从单词查找树中删除一个键（和它相关联的值）”  应改为：  我们已经考虑过的代码</td> <td>3</td>
<tr> <td>483</td>  <td>命题 G：最多的键的长度  应改为： 最多为键的长度 。</td> <td>3</td>
<tr> <td>484</td>  <td>第5行：R 中的所有  应改为： 字母表中 R 个 。</td> <td>3</td>
<tr> <td>485</td>  <td>表 5.2.2，右下角：40亿  应改为： 400万 。</td> <td>3</td>
<tr> <td>489</td>  <td>第1行：keyThatMatch()  应改为： keysThatMatch() 。</td> <td>3</td>
<tr> <td>491</td>  <td>第491页，提高题 5.2.14 和 5.2.15：唯一子字符串  应改为： 不同子字符串 。（共5处）</td> <td>3</td>
<tr> <td>492</td>  <td>实验题 5.2.24：war.txt  应改为： WarAndPeace.txt 。</td> <td>3</td>
<tr> <td>493</td>  <td>第3行： 子字符串请见图 5.3.1。  应改为：  子字符串，请见图 5.3.1。</td> <td>3</td>
<tr> <td>496</td>  <td>第3自然段，第2行： 当在文本 A A B A A *B* A A A A 中查找模式 A A *B* A A A 时  编辑说明  *B* 处的 B 应该加粗。</td> <td>3</td>
<tr> <td>496</td>  <td>倒数第5行：dfs  应改为： dfa 。</td> <td>3</td>
<tr> <td>497</td>  <td>正文第8行至第9行的代码“txt.charAt(i+1)(dfa[txt.charAt(i)][j])”左数第二个“(”和右数第一个“)”不是代码的一部分，这里的意思是txt.charAt(i+1)与dfa[txt.charAt(i)]等价。故应该采用中文全角字符，且不应采用等宽字体。</td> <td>3</td>
<tr> <td>497</td>  <td>第497页，右下角的代码框： int i, j, N = txt.length();  应改为：  int i, j, N = txt.length(), M = pat.length();</td> <td>3</td>
<tr> <td>498</td>  <td>第7行：txt.charAt(i)  应改为： pat.charAt(j) 。</td> <td>3</td>
<tr> <td>501</td>  <td>代码的最后： public static void main(String[] args) // 请见表 5.3.1  应改为：  public static void main(String[] args) // 请见下一页的“KMP子字符串查找算法的测试用例”代码框</td> <td>3</td>
<tr> <td>502</td>  <td>倒数第2行：“向右移动 5 个位置”应改为“向右移动 4 个位置”。</td> <td>3</td>
<tr> <td>505</td>  <td>代码的最后：  public static void main(String[] args) // 请见表 5.3.1   应改为：   public static void main(String[] args) // 请见第502页的“KMP子字符串查找算法的测试用例”代码框</td> <td>3</td>
<tr> <td>507</td>  <td>第7行，公式的最后部分：t i+M  编辑说明  i+M 整个都是 t 的下标</td> <td>3</td>
<tr> <td>507</td>  <td>第11行：（请见 3.1.1.4 节） 应改为： （请见 3.4.1.4 节）。</td> <td>3</td>
<tr> <td>512</td>  <td>提高题 5.3.27：“abcd” 应改为： “abcab”。</td> <td>3</td>
<tr> <td>512</td>  <td>提高题 5.3.27：”abcabcababcababcababcab“ 应改为： “abc*abcababcababcab*abcab”。  编辑说明  说明：其中 *...* 之间的字符应加粗。</td> <td>3</td>
<tr> <td>512</td>  <td>提高题 5.3.32：唯一的子字符串  应改为： 不同的子字符串 。</td> <td>3</td>
<tr> <td>517</td>  <td>倒数第4行：“*.StdIn.*” 应改为： “.*StdIn.*”。</td> <td>3</td>
<tr> <td>526</td>  <td>class GREP 的代码，以及运行结果的最后1行（共两处）： String txt = StdIn.hasNextLine();  应改为：  String txt = StdIn.readLine();</td> <td>3</td>
<tr> <td>528</td>  <td>提高题 5.4.15，第2行：(.*1)*  应改为： (0.*1)* 。</td> <td>3</td>
<tr> <td>532</td>  <td>图 5.5.3：96位  应改为： 96 bits 。（共三处）</td> <td>3</td>
<tr> <td>534</td>  <td>图 5.5.6：1 000 000位  应改为： 1000000 bits。</td> <td>3</td>
<tr> <td>534</td>  <td>倒数第4行：练习 5.4.16 和练习  应改为： 练习 5.4.16 到练习 。</td> <td>3</td>
<tr> <td>535</td>  <td>倒数第15行： 且只在最后附加32位用于记录总长度  应改为：  且附加32位用于记录总长度</td> <td>3</td>
<tr> <td>536</td>  <td>图 5.5.7： 264位  应改为： 264 bits 。（仅改程序输出的一处，第一行的标题中的不用改） 104位  应改为： 104 bits 。（两处） 50 000位  应改为： 50000 bits 。（仅改程序输出的一处，标题中的不用改） 12 536位  应改为： 12536 bits。</td> <td>3</td>
<tr> <td>537</td>  <td>图 5.5.8：1536位  应改为： 1536 bits 。</td> <td>3</td>
<tr> <td>537</td>  <td>图 5.5.8： 7 1s  应改为： 7个1，并且指向左边的箭头应再往左一点指到加粗的1的位置。 17 0s  应改为： 17个0，并且指向左边的箭头应再往左一点指到加粗的0的位置。</td> <td>3</td>
<tr> <td>538</td>  <td>倒数第2行：原来的一倍  应改为： 原来的2倍 。</td> <td>3</td>
<tr> <td>539</td>  <td>图 5.5.9 的右边：  % java PictureDump 32 36 < q32x48.rle.bin   应改为：   % java PictureDump 32 36 < q32x48.bin.rle</td> <td>3</td>
<tr> <td>539</td>  <td>图 5.5.9： 40位  应改为： 40 bits 。（两处，标题中的不用改） 32位  应改为： 32 bits 。 416位  应改为： 416 bits 。 1144位  应改为： 1144 bits 。（两处） 6144位  应改为： 6144 bits 。（两处，标题中的不用改） 2296位  应改为： 2296 bits 。（两处） 1536位  应改为： 1536 bits 。（一处，标题中的不用改）</td> <td>3</td>
<tr> <td>540</td>  <td>第17行：用了77位  应改为： 用了84位 。</td> <td>3</td>
<tr> <td>540</td>  <td>第20行：加上10个  应改为： 加上11个  。</td> <td>3</td>
<tr> <td>541</td>  <td>第541页，图 5.5.10： 图中的 压缩后的比特字符串（两处）： 0 1111 1110 0 110 0 100 0 ... - ---- ----- - --- - --- - ... A    B    R A   C A   D A ... 没有对齐。应改为对齐。</td> <td>3</td>
<tr> <td>542</td>  <td>第3行：后面框注  应改为： 左边框注 。</td> <td>3</td>
<tr> <td>543</td>  <td>第17行：如左下  应改为： 如右下 。</td> <td>3</td>
<tr> <td>545</td>  <td>图 5.5.13：就是M的编码  应改为： 就是m的编码 。</td> <td>3</td>
<tr> <td>546</td>  <td>第546页，第13行：图 5.5.13 中所显示出的空间节约  应改为： 前面讨论过的空间节约 。</td> <td>3</td>
<tr> <td>547</td>  <td>5.5.6.10 小节第1行：write-Trie()  应改为： writeTrie() 。</td> <td>3</td>
<tr> <td>548</td>  <td>图 5.5.15： 120位  应改为： 120 bits 。 352位  应改为： 352 bits 。</td> <td>3</td>
<tr> <td>549</td>  <td>图 5.5.15（续）： 45056位  应改为： 45056 bits 。 23912位  应改为： 23912 bits 。 5812552位  应改为： 5812552 bits 。 3043928位  应改为： 3043928 bits 。</td> <td>3</td>
<tr> <td>549</td>  <td>图 5.5.16： 12536位  应改为： 12536 bits 。 1144 位  应改为： 1144 bits 。 816 位  应改为： 816 bits 。 2296 位  应改为： 2296 bits 。 2032 位  应改为： 2032 bits 。</td> <td>3</td>
<tr> <td>551</td>  <td>第1行到第2行： 输出为12个  应改为： 输出为13个 总共96位  应改为： 总共104位 压缩比为82%  应改为： 压缩比为87%</td> <td>3</td>
<tr> <td>552</td>  <td>算法 5.11 的代码的第10行： st.put(”“ + (char) i, i);  应改为：  st.put("" + (char) i, i);  编辑说明  说明：全角的双引号改为半角的双引号。</td> <td>3</td>
<tr> <td>553</td>  <td>第5行：160位  应改为： 160 bits 。</td> <td>3</td>
<tr> <td>553</td>  <td>图 5.5.20 的标题： LZW 算法的扩展：特殊情况  应改为：  LZW 算法的展开：特殊情况</td> <td>3</td>
<tr> <td>553</td>  <td>倒数第12行：到值  应改为： 的值 。</td> <td>3</td>
<tr> <td>555</td>  <td>图 5.5.21： 12 536位  应改为： 12536 bits 18 232位  应改为： 18232 bits 2296位  应改为： 2296 bits 2824位  应改为： 2824 bits 5 812 552位  应改为： 5812552 bits （标题中的不用改） 3 043 928位  应改为： 3043928 bits 2 667 952位  应改为： 2667952 bits</td> <td>3</td>
<tr> <td>555</td>  <td>倒数第5行：还长  应改为： 变长 。</td> <td>3</td>
<tr> <td>556</td>  <td>第556页，练习 5.5.1：的编码结果  应改为： 的解码结果 。</td> <td>3</td>
<tr> <td>560</td>  <td>第560页，第14行：麦克斯维尔和玻尔兹曼  应改为： 麦克斯韦和玻尔兹曼 。</td> <td>3</td>
<tr> <td>561</td>  <td>倒数第3行：刚性碰撞  应改为： 弹性碰撞 。</td> <td>3</td>
<tr> <td>561</td>  <td>倒数第2行：请见图 6.0.4  应改为： 请见图 6.0.3 。</td> <td>3</td>
<tr> <td>561</td>  <td>倒数第2行到倒数第1行： 两个粒子的碰撞也是类似的，在物理上这是不严密的，但要更加复杂一些（请见练习 6.1）。  应改为：  两个粒子的碰撞也是类似的，但要更加复杂一些（请见练习 6.1）。</td> <td>3</td>
<tr> <td>561</td>  <td>图 6.0.4 的标题：粒子和墙体  应改为： 粒子之间 。</td> <td>3</td>
<tr> <td>562</td>  <td>第3行：请见图 6.0.5  应改为： 请见图 6.0.7 。</td> <td>3</td>
<tr> <td>562</td>  <td>第8行：忽略请见图 6.0.6  应改为： 忽略 。</td> <td>3</td>
<tr> <td>562</td>  <td>第11行：操作，请见图 6.0.7  应改为： 操作 。</td> <td>3</td>
<tr> <td>564</td>  <td>第7行到第8行：它的实现如后面框注所示  应改为： 它的实现如上一页右下角的框注所示 。</td> <td>3</td>
<tr> <td>565</td>  <td>第5行： { /* 请见正文 *// }  应改为：  { /* 请见正文 */ }</td> <td>3</td>
<tr> <td>566</td>  <td>第8行到第9行： else if (a != null && b == null) a.bounceOffHorizontalWall();   else if (a == null && b != null) b.bounceOffVerticalWall();    应改为：    else if (a != null && b == null) a.bounceOffVerticalWall();   else if (a == null && b != null) b.bounceOffHorizontalWall();</td> <td>3</td>
<tr> <td>567</td>  <td>第14行：不断前进  应改为： 不断发展 。</td> <td>3</td>
<tr> <td>567</td>  <td>倒数第3行：B-树中请见图 6.0.8  应改为： B-树中（请见图 6.0.8）。</td> <td>3</td>
<tr> <td>567</td>  <td>倒数第2行：键-接  应改为： 键-链接 。</td> <td>3</td>
<tr> <td>568</td>  <td>图 6.0.8： 左下角的：内部的 3-结点  应改为： 外部的 3-结点 。 右上角的：外部的 3-结点  应改为： 内部的 3-结点 。 中间的：每个红色的键  应改为： 每个加粗的键 。</td> <td>3</td>
<tr> <td>568</td>  <td>倒数第3行：6-结点结点  应改为： 6-结点 。</td> <td>3</td>
<tr> <td>569</td>  <td>图 6.0.10： 图的连线有误。  编辑说明  请参见：http://www.ituring.com.cn/article/36750</td> <td>3</td>
<tr> <td>569</td>  <td>倒数第2行： API 中的“打开”（open）和“关闭”（close）方法指的是  应改为：  API 中的术语“打开”（open）和“关闭”（close）指的是</td> <td>3</td>
<tr> <td>569</td>  <td>最后1行到第570页第1行： add() 方法是为内部页准备的，它是一个符号表操作  应改为：  内部页的 add() 方法是一个符号表操作 第570页，第1行到第2行： add() 和 contains() 方法是为外部页准备的，和 SET 中相应的方法类似。  应改为：  外部页的 add() 和 contains() 方法和 SET 中相应的方法类似。</td> <td>3</td>
<tr> <td>570</td>  <td>第7行：用网页实现 Page  应改为： 实现 Page 用于网页。</td> <td>3</td>
<tr> <td>571</td>  <td>第6行：一倍  应改为： 两倍 。</td> <td>3</td>
<tr> <td>571</td>  <td>算法 6.12  应改为： 算法 6.1 。</td> <td>3</td>
<tr> <td>571</td>  <td>算法6.12 B-树集合的实现： 这个算法的代码中的所有 put 都应改为 add，共七处： put(sentinel); put(root, key); root.put(lefthalf); root.put(righthalf); if (h.isExternal()) { h.put(key); return; } put(next, key); h.put(next.split());  应改为：  add(sentinel); add(root, key); root.add(lefthalf); root.add(righthalf); if (h.isExternal()) { h.add(key); return; } add(next, key); h.add(next.split());</td> <td>3</td>
<tr> <td>573</td>  <td>倒数第12行到倒数第11行： 将一个字符串中起始位置为 i 的子字符串与另一个字符串中起始位置为 j 的子字符串相比较  应改为：  将字符串中每个起始位置为 i 的子字符串与另一个起始位置为 j 的子字符串相比较</td> <td>3</td>
<tr> <td>575</td>  <td>倒数第3行：方法、select() 倒数第2行：索引值、lcp() 倒数第1行：前缀、rank() 这里的三个顿号（、）应改为逗号（，）。</td> <td>3</td>
<tr> <td>576</td>  <td>第11行：在右边框注所示的例子中  应改为： 在图 6.0.15 所示的例子中 。</td> <td>3</td>
<tr> <td>577</td>  <td>倒数第3行：算法 3.2（续） 应改为： 算法 3.2（续1）。</td> <td>3</td>
<tr> <td>577</td>  <td>倒数第10行：算法 6.13  应改为： 算法 6.2 。</td> <td>3</td>
<tr> <td>578</td>  <td>算法 6.13  应改为： 算法 6.2 。</td> <td>3</td>
<tr> <td>578</td>  <td>算法 6.13： // 请见 6.0.3.2 节框注“两个字符串的最长公共前缀” 这行之前需要增加以下一行： private static int lcp(String s, string t)</td> <td>3</td>
<tr> <td>582</td>  <td>第4行：命题 C  应改为： 命题 E 。</td> <td>3</td>
<tr> <td>582</td>  <td>倒数第7行：WeightedEdge  应改为： Edge 。</td> <td>3</td>
<tr> <td>582</td>  <td>倒数第6行：WeightedDirectedEdge  应改为： DirectedEdge 。</td> <td>3</td>
<tr> <td>582</td>  <td>倒数第1行：WeightedEdge  应改为： EdgeWeightedGraph 。</td> <td>3</td>
<tr> <td>582</td>  <td>倒数第6行：但 FlowEdge 的基类并不是  应改为： 但 FlowEdge 并不是基于 。</td> <td>3</td>
<tr> <td>582</td>  <td>检查流量网络中的一种流量配置是否可行 代码框，倒数第8行：e.cap()  应改为： e.capacity() 。</td> <td>3</td>
<tr> <td>582</td>  <td>第582页，代码框中的第二行： {   // 检查每个顶点v的局部平衡  应改为：  {   // 检查顶点v的局部平衡</td> <td>3</td>
<tr> <td>583</td>  <td>第2行：框注  应改为： 上一页框注 。</td> <td>3</td>
<tr> <td>583</td>  <td>表 6.0.4，倒数第2行：addFlowTo  应改为： addResidualFlowTo 。</td> <td>3</td>
<tr> <td>584</td>  <td>图 6.0.21 的第3幅0-2线应为全灰。  编辑说明  请参见：http://www.ituring.com.cn/article/36800</td> <td>3</td>
<tr> <td>585</td>  <td>第15行到第16行： 切分会从入口流向出口的原油完全切断  应改为：  一个切分提供了将从入口流向出口的原油完全切断的方法</td> <td>3</td>
<tr> <td>588</td>  <td>正文第一行 residualCapacityTo() 和 residualFlowTo() 方法实现了剩余网络。  应改为：  residualCapacityTo() 和 addResidualFlowTo() 方法实现了剩余网络。</td> <td>3</td>
<tr> <td>589</td>  <td>第589页，第1行和第4行：算法 6.14  应改为： 算法 6.3 。（共两处）</td> <td>3</td>
<tr> <td>594</td>  <td>第6行：优先级调度示例问题  应改为： 优先级限制下的并行任务调度问题 。</td> <td>3</td>
<tr> <td>595</td>  <td>图 6.0.25：该图中的第2幅图忘了把最大流量配置的边涂成灰色。  编辑说明  参见本书英文版第906页。</td> <td>3</td>
<tr> <td>595</td>  <td>倒数第15行：4-7 和 6-11  应改为： 4-7、5-10 和 6-11 。</td> <td>3</td>
<tr> <td>595</td>  <td>图 6.0.25：这幅图中的第1幅图和第2幅图的终点（在最下方）的名称都应改为 t，而不是 s 。</td> <td>3</td>
<tr> <td>596</td>  <td>命题 K 的 例证，第1行：练习 6.49  应改为： 练习 6.50 。</td> <td>3</td>
<tr> <td>596</td>  <td>图 6.0.26：该图中的最后一幅图忘了把最大流量配置的边涂成灰色。  编辑说明  英文版第907页</td> <td>3</td>
<tr> <td>598</td>  <td>倒数第2行：前面框注  应改为： 后面框注 。</td> <td>3</td>
<tr> <td>598</td>  <td>倒数第1行：有向图  应改为： 图 。</td> <td>3</td>
<tr> <td>599</td>  <td>倒数第4行：在 6.0.6.5 节  应改为： 在 6.0.6.6 节 。</td> <td>3</td>
<tr> <td>601</td>  <td>表 6.0.7，最后1行：请见表 6.0.7  应改为： 请见表 6.0.8 。</td> <td>3</td>
<tr> <td>604</td>  <td>第20行：找出它的最大因数  应改为： 找出它的一个非平凡因数 。</td> <td>3</td>
<tr> <td>605</td>  <td>倒数第1行：1.3806503  应改为： 1.3806488 。</td> <td>3</td>
<tr> <td>608</td>  <td>练习 6.31：Burrow-Wheeler  应改为： Burrows-Wheeler 。（共4处）</td> <td>3</td>
<tr> <td>608</td>  <td>练习 6.31，倒数第2行：逆变换是  应改为： 逆变换（BWI）是 。</td> <td>3</td>
<tr> <td>609</td>  <td>练习 6.42：用练习 6.42 中  应改为： 用练习 6.41 中 。</td> <td>3</td>
<tr> <td>609</td>  <td>练习 6.49：最大因数  应改为： 一个非平凡因数 。</td> <td>3</td>
<tr> <td>611</td>  <td>索引，右栏，第15行：Aliasing  应改为： Aliasing（别名）。</td> <td>3</td>
<tr> <td>611</td>  <td>索引，右栏，第16行：of arrays（别名）  应改为： of arrays（数组）。</td> <td>3</td>
<tr> <td>611</td>  <td>索引，右栏，第18行：of substrings（子数组）  应改为： of substrings（子字符串）。</td> <td>3</td>
<tr> <td>614</td>  <td>索引，左栏，C 字头前面1项：原书数据类型  应改为： 原始数据类型 。</td> <td>3</td>
<tr> <td>614</td>  <td>索引，右栏，第3行：认证  应改为： 证明 。</td> <td>3</td>
<tr> <td>615</td>  <td>索引，右栏，第25行：见最短路径算法  应改为： 见关键路径算法 。</td> <td>3</td>
<tr> <td>615</td>  <td>索引，右栏，第30行：关键路径法  应改为： 关键路径算法 。</td> <td>3</td>
<tr> <td>617</td>  <td>索引，左栏，倒数第14行：拓补排序  应改为： 拓扑排序 。</td> <td>3</td>
<tr> <td>617</td>  <td>索引，右栏，第14行到第18行：这5行应该整体左移2格，向本栏第1行看齐。</td> <td>3</td>
<tr> <td>617</td>  <td>索引，右栏，倒数第10行：加权有向图  应改为： 无环加权有向图 。</td> <td>3</td>
<tr> <td>618</td>  <td>索引，左栏，第27行：欧几里德算法  应改为： 欧几里得算法 。</td> <td>3</td>
<tr> <td>618</td>  <td>索引，右栏，倒数第22行：向上取整函数  应改为： 向下取整函数 。</td> <td>3</td>
<tr> <td>622</td>  <td>索引，右栏，第19行：ConcurrentModification  应改为： ConcurrentModificationException 。</td> <td>3</td>
<tr> <td>622</td>  <td>索引，K 字头前面1项：JIT 编辑器  应改为： JIT 编译器 。</td> <td>3</td>
<tr> <td>625</td>  <td>索引，左栏，倒数第1行：该行必须右移2格。</td> <td>3</td>
<tr> <td>625</td>  <td>索引，右栏，倒数第11行：向上取整和向下取整函数  应改为： 向下取整和向上取整函数 。</td> <td>3</td>
<tr> <td>626</td>  <td>索引，左栏，第9行：过载  应改为： 重载 。</td> <td>3</td>
<tr> <td>626</td>  <td>索引，右栏，第18行：Kendall's tau 距离  应改为： Kendall tau 距离 。</td> <td>3</td>
<tr> <td>627</td>  <td>索引，左栏，第5行：对于无向图  应改为： 对于有向图 。</td> <td>3</td>
<tr> <td>627</td>  <td>索引，左栏，倒数第16行：演算法  应改为： 概率算法 。</td> <td>3</td>
<tr> <td>629</td>  <td>第629页，索引，左栏，第8行：最大流消减  应改为： 最大流归约 。</td> <td>3</td>
<tr> <td>629</td>  <td>索引，左栏，倒数第14行：拓补排序  应改为： 拓扑排序 。</td> <td>3</td>
<tr> <td>629</td>  <td>索引，右栏，倒数第18行：拉斯维佳斯  应改为： 拉斯维加斯。</td> <td>3</td>
<tr> <td>630</td>  <td>索引，左栏，倒数第16行：线性归划  应改为： 线性规划 。</td> <td>3</td>
<tr> <td>630</td>  <td>索引，右栏，第13行：完整的比较序列  应改为： 全序关系 。</td> <td>3</td>
<tr> <td>630</td>  <td>索引，右栏，倒数第2行：立方级别  应改为： 平方级别 。</td> <td>3</td>
<tr> <td>630</td>  <td>索引，右栏，第22行：  Reverese postorder traversal  应改为：   Reverse postorder traversal  并将该索引条目后移到第31行。</td> <td>3</td>
<tr> <td>632</td>  <td>索引，右栏，第3行：rul  应改为： rule 。</td> <td>3</td>
<tr> <td>633</td>  <td>索引，右栏，倒数第19行：向上取整和向下取整  应改为： 向下取整和向上取整 。</td> <td>3</td>
<tr> <td>634</td>  <td>索引，左栏，倒数第17行：拓补排序  应改为： 拓扑排序 。</td> <td>3</td>
<tr> <td>634</td>  <td>索引，左栏，倒数第13行：完整比较序列  应改为： 全序关系 。</td> <td>3</td>
<tr> <td>948</td>  <td>INDEX，第2栏，倒数第12行：   Reverese postorder traversal  应改为：    Reverse postorder traversal   并将该索引条目后移到倒数第2行。  这就是中文版的勘误呀，为什么退回？对应的英文版勘误本书作者 Kevin Wayne 已经确认了。 哦，对不起，这是英文版的页码。</td> 
</table>
