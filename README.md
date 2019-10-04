# Operation-Analysis
for self-developing

## Statistics For Business And Economics-Note
### 统计、数据和统计思维
#### 定义
**描述统计** 指利用数字或者图表的方法，寻找数据的规律，总结其中的信息，并以恰当的方式展示。

**推断统计** 指利用样本数据的信息，对总体的情况做出估计、推断和预测。

**总体** 是我们所关心的全体单元的集合。

**试验单元** 是我们采集数据的对象。

**变量** 是每个试验单元的特征或属性。

**样本** 是总体的一个子集。

**可靠性测量** 是对统计推断结果的不确定性程度定量的陈述。

**黑箱** 是指操作或行为未知或不明确的过程。

**定量数据** 用数值尺度记录。

**定性数据** 仅仅能被分成不同的类别。

**简单随机样本** 是指在一个总体中所有样本量为n的样本都有相同的机会被抽中时，所抽取的其中某一个样本。

**分层随机抽样** 当同层内的试验单元比不同层间的试验单元更具相似性，一般使用分层随机抽样。分层随机抽样指从各层中抽取一定数量的元素组成一个完整的样本。

**系统抽样** 这种方法是指从所有试验单元中每隔k个抽取1个试验单元。

**随机响应问题** 当受访者很容易不给出真实答案时。

**选择偏差** 导致总体的一个样本子集在抽取样本时被排除，该样本中的个体无法被抽中。

**无应答偏差** 导致被选中的样本中，并非所有试验个体都参与了调查。

**测量误差** 测量数据的不精确。

#### 概念
1. > 统计涉及两个不同的阶段：描述数据集（**描述统计**）和根据样本信息得出结论（**推断统计**）。
2. > 描述统计的四个要素：样本或总体、变量、图表或其他总结工具、数据规律的确定。
2. > 推断统计问题五个要素：**总体**、**变量**、**样本**、**推断**和**可靠性(reliability)**。
3. > 随机抽样设计方法：**简单随机抽样**、**分层随机抽样**、**整群抽样**、**系统抽样**、**随即响应抽样**

#### 结论
1. 为了进行统计推断，我们须获得有代表性的样本。

#### Q&A
1. 分层抽样和整群抽样有何区别？
![Alt text](https://pic2.zhimg.com/1546ac4bd52323e6f508edb9e9a98dab_r.jpg)


### 数据集的描述方法
#### 定义
**帕累托直方图** 
**集中趋势** 也就是测度数据聚集的趋势或某些数值的中心
**变异性** 也就是测度数据的分散状况
**偏态** 如果分布的一个尾部比另一尾部具有更多的极端观测值，则数据集被认为是偏态的。

#### 概念
1. > 帕累托原理(大概是说)：社会总财富的80%掌握在20%的家庭中。“至关重要的少数和微不足道的大多数”。
2. > 数值描述测度：数据的集中趋势测度，数据的变异性测度。

#### 公式
1. ![](http://latex.codecogs.com/gif.latex?\barx=\frac{\sum_{i=1}^n x_i}{n})
2. ![](http://latex.codecogs.com/gif.latex?\barx) 是样本均值；![](http://latex.codecogs.com/gif.latex?\mu) 是总体均值。

#### 结论
1. 一般来说，极端值（更大或更小）对均值的影响要大于中位数。
2. 右偏数据通常会显示出均值大于中位数。

#### Q&A

## numpy中的方差、协方差、相关系数
### 方差 np.var
np实际上是均方差，与方差不太一样，均方差就是把方差平均化。
np.std是标准差，np.std²=np.var
无论是方差还是标准差，它们衡量的都是二阶中心距。
### 协方差 np.cov
方差是特殊的协方差, D(X) = cov(X, X)
协方差表示的是两个向量的关联程度，其实相当于：把两个向量中的变量进行中心化（减去均值），然后计算剩余向量的內积。
np.cov和协方差不太一样，在无偏估计下：np.cov = cov/(n-1);在有偏估计情况下，np.cov = cov/n
### 相关系数 np.correlate
np.cov描述的是两个向量协同变化的程度，它的取值可能非常大，也可能非常小，这就没法直观的衡量二者协同变化的程度，而相关系数其实是正则化的协方差。

## Reference Material
- [使用过Spotfire的朋友，可否分析下优缺点](https://www.zhihu.com/question/41444381)
- [matplotlib官方](https://matplotlib.org/)
- [numpy中的方差、协方差、相关系数](https://www.cnblogs.com/weiyinfu/p/10693445.html)
