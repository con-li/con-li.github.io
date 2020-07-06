---
layout: post
title: 模型建立、调优流程入门
author: Cong Li
date: 2018-08-29 08:08:17
header-style: text
tags:
- 数据科学
- 知识规划
- 模型生成
---
### 1. 模型建立

基于optimization theory，定义loss function，搜索parameter

  * 模型类型 
      * 统计模型 
          * 分类器：有监督，SVM, LR, DT；无监督，K-means, K-means++, ISODATA, GMM, SOM
          * 回归器：GLR
          * 时序模型：ARIMA，GARCH
      * 神经网络 
          * 基本DNN：CNN，常用ResNet; RNN，常用LSTM
          * 强化学习
          * 迁移学习
          * GANs
      * 知识图谱，基于概率图模型
  * 模型融合-Ensemble learning 
      * Bagging: Random Forest
      * Boosting: GBDT, popular used as XGBoost

### 2. 模型调优

基于optimization theory，定义loss function，搜索hyperparameter

  * 模型评估 
      * 线下 
          * 评估方式：hold-out, k-fold
          * 准确率指标：AUC, F1, Accuracy, Recall, RMSE
      * 线上 
          * 评估方式: AB test
          * 活客、黏客、转化率、客单价提升
  * 参数调优 
      * 类型：模型先验参数、网络层和神经元、图谱节点和边
      * 搜索方法: Grid, Random, Bayesian