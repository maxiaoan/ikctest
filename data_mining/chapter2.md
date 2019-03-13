# Data Preprocessing
### Data Cleansing
#### Why Data Preprocessing
- Real data arenotoriously dirty
- Incomplete
- Noisy
- Inconsistent
- Redundant
- Others
  - Data types 
  - Imbanlanced datasets
#### Missing Data
##### Data are not always available.
- One or more attributes of a sample may have empty values.
- Many data mining algorithms cannot handle missing values directly.
- May cause significant troubles.

##### Possible Reasons
- Equipment malfunction 设备故障
- Data not provided 数据未提供
- Not Applicable (N/A) 不可用

##### Different Types
- Missing completely at random 完整数据随机缺失
- Missing conditionally at random 有条件的随机缺失
- Not missing at random 

##### How to handle missing data
- Ignore
- Fill in the missing values manually
- Fill in the missing values automatically
- More art than science

Outliers 离群值
Anormaly 异常值
- Local Outlier Factor 局部偏离因子
Duplicate Data


### Data Transformation
Now we have an error free dataset. Still needs to be standardized.
#### Data Attribute Types
- Continuous 连续型
  - Real values
- Discrete 离散型
  - number of people,
- Ordinal 序数型
  - Rankings:{Average, good, best}
- Norminal 标称型
  - Symbols:{Teacher, Worker, Salesman}
- String
  - Text: {Tsinghua university}

#### Type Conversion
  - 颜色的编码
#### Normalization
#### Sampling
A database/data warehouse may store terabytes of data.

- Processing limits: CPU, Memory, I/O …

- Sampling is applied to reduce the **time complexity**.

In statistics, sampling is applied often because obtaining the entire set of data is expensive.

- Aggregation
 - Change of scale:   缩小问题规模
  - Cities -> States;
  - Days -> Months
 - More stable and less variability 提高稳定性

- Sampling can be also used to adjust the class distributions.
  - Imbalanced dataset 数据集的不平衡
- OverSapmping 
  - Synthetic Minority OverSampling Technique
  - 合成少数类过采样技术,对少数类样本通过插值进行上采样
- Boundary Sampling
  - 极度不平衡的二分类数据集采用**边界采样**,提高少数样本的准确率

#### Normalization
- Min-max normalization:
  - Let income range $12,000 to $98,000 be normalized to [0.0, 1.0].  Then $73,600 is mapped to  
    - (73600-12000)/(98000-12000)*(1.0 -0 ) + 0 = 0.716
    > 注:有明确上下界，映射到[0, 1] 区间
- Z-score normalization (μ: mean, σ: standard deviation):
	- 距离平均值的标准差

### Data Description
- Mean
- Median
- Mode
- Variance
- Pearson’s product moment correlation coefficient(皮尔森积矩相关系数)
- Pearson's chi-square (χ2) test 皮尔逊的卡方测试
#### Data Visualization
- 1D 
  - 饼图，柱状图，散点图, 直方图
- 2D
  - 直角坐标
- 3D
  - Surf Plot 
- High Dimensional
  - Box Plot
  - Parallel Coordinates
##### Software for Visulization
 - CiteSpace
 - Gephi
### Feature Selection
- Class Distributions
- Entropy量化（熵）
  - 熵用来衡量系统的不确定性（熵越小越好）
  - Information Gain信息增益
    - 原始的熵 - 附加属性之后的熵 = 信息增益
    - 知道某个属性，可以降低系统预测信息的不确定性，信息增益数值越大越好，可以降低系统不确定的幅度
- Feature Subset Search
  - Exhaustive 
  - All possible combinations 枚举组合
  - Branch and Bound 分支定界（最优解）
  - Top K Individual Features
  - Sequential Forward Selection（前向选择法）
  - Sequential Backward Selection（顺序后退法）
  - Optimization Algorithms
	- Simulated Annealing模拟退火算法
	- Tabu Search禁忌搜索算法
	- Genetic Algorithms遗传算法

### Feature Extraction
- 特征提取包含特征选择
#### 1. Principal Component Analysis
- Data: Gaussian Distribution
- Variance差值，即为主要的属性: Information（所要提取的成分）
- Ellipse(椭圆): Major Axis(长轴) vs. Minor Axis(短轴)
  - Select the attribute corresponding to the Major Axis.
- Lagrange Multipliers(拉格朗日乘数法计算最优解)
- **PCA** To project the original data to the eigenvectors（特征向量） of S with the largest eigenvalues（特征值）.
将原始数据投影到特征向量上；其中，特征向量为特征值最大（多个）的那些特征向量（特征向量需要从大到小排序）
- 尽量将数据投影到数据散布大的方向
- PCA 变换包括去均值、矩阵特征值分解、坐标变换
- The Issue of PCA is losing class information
- 可将数据降到1 到 n-1维
#### 2. Linear Discriminant Analysis 线性判别分析
- The objective of LDA is to perform dimension reduction while preserving as much of the class discriminatory(类区分信息)information as possible.
- maximizes the separability
- Fisher Criterion （fisher准则）
  - Maximize the distance between classes
  - Minimize the scatter within each class
- Limitations of LDA
  - LDA produces at most C-1 projections, SB is a matrix with rank C-1 or less.
  - SW may be singular.
  - LDA does not work well when u1= u2，均值若相等，Fisher的数值为0

### Reading Materials
M. A. Hernandez and S. J. Stolfo, “Real-World Data is Dirty: Data Cleansing and The Merge/Purge Problem,” Data Mining and Knowledge Discovery, vol. 2, pp. 9–37, 1998.

A. Donders, G. van der Heijden, T. Stijnen, and K. Moons, “Review: A Gentle Introduction to Imputation of Missing Values,” Journal of Clinical Epidemiology, vol. 59, pp. 1087-1091, 2006.

N. V. Chawla, K. W. Bowyer, L. O. Hall and W. P. Kegelmeyer, “SMOTE: Synthetic Minority Over-Sampling Technique,” Journal of Artificial Intelligence Research, vol. 16, pp. 321–357, 2002.

N. Japkowicz and S. Stephen, “The Class Imbalance Problem: A Systematic Study,” Intelligent Data Analysis, vol. 6, pp. 429–449, 2002.

D. Keim, “Information Visualization and Visual Data Mining,” IEEE Transactions on Visualization and Computer Graphics, vol. 8, pp. 1-8, 2002.

PCA Tutorials
http://www.cs.princeton.edu/picasso/mats/PCA-Tutorial-Intuition_jp.pdf
http://www.cs.otago.ac.nz/cosc453/student_tutorials/principal_components.pdf 

Lagrange Multipliers
http://diglib.stanford.edu:8091/~klein/lagrange-multipliers.pdf




