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
- Outliers 离群值
- Anormaly 异常值
- Local Outlier Factor 局部偏离因子
-  Duplicate Data


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
  - Cities  States;
  - Days  Months
 - More stable and less variability 提高稳定性

- Sampling can be also used to adjust the class distributions.
 - Imbalanced dataset 数据集的不平衡

### Data Description

### Feature Selection

### Feature Extraction



