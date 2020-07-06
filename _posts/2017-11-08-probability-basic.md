---
layout: post
title: 概率论基础
author: Cong Li
date: 2017-11-08 03:11:11
header-style: text
tags:
- 数据科学
- 知识规划
- 概率论
---
### 1. 样本空间 i.i.d观测



### 2. 样本空间-概率空间的映射->分布

  * 分布类型 
      * 单变量 
          * 连续，uniform, exponential, Gaussian, chi-square, T, F
          * 离散，Bernoulli, binomial, Poisson
      * 多变量：联合分布，边缘分布是单变量分布
  * 分布特征 
      * 单变量-矩：mean, var, skewness, kurtosis
      * 多变量：cov, cor

### 3. 样本空间子集->事件，事件映射到概率空间的测度->概率

  * 频率观点：频率逼近概率，预估-MLE
  * 贝叶斯观点：新观测+先验概率=后验概率，预估-MAP 
      * MAP with Gaussian prior=MLE+L2 regularization

### 4. 已观测的发生事件->样本

  * 中心极限+大数
  * 点估计：标准，无偏、有效、一致
  * 区间估计，对偶假设检验