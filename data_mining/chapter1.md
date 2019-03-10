---
」typora-root-url: ./picture
---

# Data Mining: Theory & Algorithms

## 1. Technology Advancement
- Data storage has grown significantly，shift markedly from analog digital after 2000
- Computing capacity has also risen sharply	

## 2. The World of Data 
- social networks
- future goods
- mobile phone
- credit card
- health and financial
## 3. Data Rich，Pnformation Poor（DRIP）

## 4. Learning  Resources
- 《Data minning》
  -《模式分类》
- 《beautiful data》
- 国际知名的期刊和会议

  - International Conference on Data Mining
  - International Conference on Data Engineering
  - International Conference on Machine Learning
  - International Joint Conference on Artificial Intelligence
  - Pacific-Asia Conference on Knowledge Discovery and Data Mining
  - ACM SIGKDD Conference on Knowledge Discovery and Data Mining
  - 科学研究只有第一，没有第二。掌握最新动态
- Tools工具
  - 搜文章用Google，Google学术，
  - UCI machine learning repository
  - WEKA software 数据挖掘软件
  - MATLAB中的数据挖掘软件包

## 5. Interdisciplinary (跨学科)

- Data mining 
  - Artificial Intelligence
  - Machine Learning
  - Pattern Recognition
  - Statistics

### 6. Ubiquitous(普适计算)

- Data Mining
  - Decision support
  - Business Intelligence
  - Data Analytics
  - Customer Relationship Management
  - Big Data

### 7. Comprehensive Learning

- Class Teaching
  - Thinking
  - DIscussion
- Reading Materials
  - Extension
  - Inspiration

- Practice
  - Techniques
  - Applications

### 8. Data

> **Data definition**
> Data are pieces of information that represent the qualitative or quantitative attributes of a variable or set of variables. Data are often viewed as the lowest level of abstraction from which information and knowledge are derived.”

- **Data Type**
  - Continuous，Binary
  - Discrete，String
  - Symbolic

- Storage Type
  - Physical
  - Logical
- Major Issue
  - Transportation
  - Errors and Corruption

### 9. Big Data

> **Big data** is **high-volume**, **high-velocity** and **high-variety** information assets that demand cost-effective, innovative forms of information processing for enhanced insight and decision making.”  

#### 大数据的应用
- public security
- Health Care  and Application
  - overtreatment
  - undertreatment
  - personalized medicine
- Location Data
  - urban planning 
  - Mobile Data
  - Shoper via RFID
- Retail Data
  - targeted marketing(Customer service)目标客户
  - sentiment analysis(comments) 情感分析
- social Networks
- Sports 
  - 《money ball》
- attractiveness Mining （魅力挖掘）



### 10. Open data 
- technical open
- legally open
- open government data

### 11. Data mining

- Statistics

  - Mean, Variance, Correlation, Distribution 

- Definition

  - Data Mining is the process of automatically extracting **interesting** and **useful** **hidden** patterns from usually **massive**, incomplete and noisy data.

    

- Not a fully automatic process

  - Human interventions are often inevitable.
  - Domain Knowledge
  - Data  Collection and Pre-processing

- synonym: knowledge discovery

### 11. Is DM really important？

- business intelligence

#### From data to Knowledge

```mermaid
graph LR
Data --> Information --> Knowledge --> Decision support 
Database --> Preprocessing --> Data mining --> Decision models
```

#### Data integration & Analysis

- From ERP、CRM、Flat files through **ETL** to Data  warehouse  and then Data Mining.

![dataintegration](/Users/maxiaoan/ikctest/data_mining/picture/dataintegration.png)

**ETL:**  stands for extraction, transportation, loading

#### The process of data mining

![processing of data](/Users/maxiaoan/ikctest/data_mining/picture/processing of data.png)

#### Data Ming software

- IBM SPSS
- SAP predictive analysis
- Fall

### 12. Classification Problem

#### DM techniques-classification

- ##### Algorithm

  - decision tree 决策树
  - K-nearest neighbours（KNN）
  - neural networks神经网络
  - support vector machine 向量机

- Application

  - Churn Prediction 流失预测
  - Medical Diagnosis 医疗诊断

  ##### classification boundaries	分类边界

  - 收入与存款

  ##### overfitting -classification

  - 过渡拟合

  ##### cross validation（交叉验证）

  - data 
    - training set 产生模型
    - Test set  测试模型，并反馈给训练集并继续优化

##### confusion Matrix

![confusion matrix](/Users/maxiaoan/ikctest/data_mining/picture/confusion matrix.png)

- TPR = TP/(TP + FN)	

- TNR = TN/(TN + FP)

- TNPR = (TP + TN)/(TP + TN + FN +FP) 

  ##### ReceiverOperating Characteristic
  - Area Under Curve 曲线越高越好，上限为1
  - 模型小于50%，即小于ramdom Guess 则无法使用，random Guess
  - Cost sensitive learning 
  - lift analysis 电梯客流分析
  - waterfall analysis

#### DM Techniques - Clustering

>  **Clustering** is the assignment of a set of observations into subsets (called *clusters*) so that observations in the same cluster are similar in some sense

#### clustering and other data Mining Problems

- clustering 聚类

- distance metrics
	- euclidean distance （欧氏距离）
	- Manhattan distance  (曼哈顿距离)
	- mahalanobis distance （马氏距离）


- Algorithm 
  - K-means（K值聚类算法）
  - Sequential Leader （顺序引导）
  - hierarchical clustering（层次聚类）
  - Affinity Propagation 近邻传播算法
- Application

  - Market Research 市场调研
  - Image Segmentation 图像分割
  - Social Network Analysis 社交网络

#### DM Technique - Association rules 关联规则

#### DM Technique - regression关联规则


- regression 回归
  备注：线性相关，是指参数与变量之间是线性的拟合。非最后的表达式的结果是线性的
- Overfitting – Regression
- performance dashboard
- data preprocessing
- Seeing is Knowing

### Data Preprocessing

Real data are often surprisingly dirty. A Major Challenge for Data Mining

1. **Typical Issues**

   * Missing Attribute Values

   * Different Coding/Naming Schemes

   * Infeasible Values

   * Inconsistent Data

   * Outliers 野值性

2. **Data Quality**

   * Accuracy

   * Completeness

   * Consistency

   * Interpretability 解释性

   * Credibility

   * Timeliness 时效性

3. **Data Cleaning**

   * Fill in missing values.

   * Correct inconsistent data.

   * Identify outliers and noisy data. 鉴别野值和噪声数据

4. **Data Integration**

   * Combine data from different sources. 数据整合

5. **Data Transformation**

   * Normalization 规范化
   * Aggregation 聚合性
   * Type Conversion 类型转换

6. **Data Reduction**

   * Feature Selection

   * Sampling

### privacy protection and parallel  computing

- cloud computing 


- parallel computing

- The big picture 

- 数据、算法、计算平台

* 原则：处理问题先从简单的算法开始，能解决问题即可
* Pay As You Go
* Software as a Service
* Platform as a Service
* Infrastructure as a Service

