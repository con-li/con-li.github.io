---
layout: post
title: 推荐系统的项目实践
author: 
date: 2018-09-30 12:09:22
header-style: text
tags: 
- 数据科学
- 生命体验
- 推荐系统
---
### 1. BRD-定位

  * 短期，流量变现，注册/登陆-点击-交易-成交-复购
  * 长期，优质信息分发

### 2. MRD-信息流

  * 匹配客户偏好
  * 识别优质信息

### 3. PRD-算法方案

  * 召回：KNN, TF-IDF, Item2Vec
  * 排序：NB, LR, GBDT(Xgboost), RippleNet, Wide&Deep
  * 过滤：领域规则
  * 补位：热销+冷门

### 4. R&D-研发部署

  * 原型：算法原型，架构原型
  * serving：联机计算，近线更新，离线准备

### 5. Tuning-调参方案

  * 评估：线下CTR预估，线上AB测试
  * 具体方案另文再述