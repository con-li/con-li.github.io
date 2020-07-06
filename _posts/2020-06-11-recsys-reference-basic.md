---
layout: post
title: 推荐系统算法参考文献入门清单
author: Cong Li
date: 2020-06-11 12:06:44
header-style: text
tags:
- 数据科学
- 知识规划
- 推荐算法
- 参考文献
---
### 1. 综述

三本参考书，建立知识框架。

  [1]项亮. (2012). 推荐系统实践［Ｍ］.人民邮电出版社

  [2]Ricci, Francesco and Rokach, Lior and Shapira, Bracha. (2011). Recommender Systems Handbook [M] , Springer

  [3]Aggarwal, Charu C. (2016). Recommender Systems:The Textbook [M] . Springer.

### 2. 召回

协同过滤，包括亚马逊最早的商品推荐专利

  [1]Linden et al. (2001). Collaborative recommendations using item-to-item similarity mappings. Amazon.

  [2]Sarwar B M and Karypis G and Konstan J A et al. (2001). Item-based collaborative filtering recommendation algorithms[J]. the Web Conference, 2001: 285-295.

  矩阵分解

  [3]Y. Koren, R. Bell and C. Volinsky. (2009). Matrix Factorization Techniques for Recommender Systems. Computer, vol. 42, no. 8, pp. 30-37, Aug. 2009.

  向量化, word2vec

  [4]Le V Q and Mikolov T. (2014). Distributed Representations of Sentences and Documents. arXiv preprint arXiv: 1405.4053

阿里开源的TDM

[5]Zhu H and Li X and Zhang P et al. (2018). Learning Tree-based Deep Model for Recommender Systems. arXiv preprint arXiv: 1801.02294

### 3. 排序

深度学习，阿里开源的Wide&Deep和华为开源的DeepFM

  [1]Cheng H and Koc L and Harmsen J et al. (2016). Wide & Deep Learning for Recommender Systems. arXiv preprint arXiv: 1606.07792

  [2]Huifeng G and Ruiming T and Yunming Y et al. (2017). DeepFM: A Factorization-Machine based Neural Network for CTR Prediction. arXiv preprint arXiv: 1703.04247

  知识图谱，美团开源的RippleNet

  [3]Wang H and Zhang F and Wang J et al. (2018). RippleNet: Propagating User Preferences on the Knowledge Graph for Recommender Systems. arXiv preprint arXiv: 1803.03467

  模型融合，Boosting集成，包括GBDT和XGBoost

  [4]Friedman J H. (2001). Function approximation: a gradient boosting machine. Annals of Statistics, 29 (5): 1189-1232, 2001

  [5]Chen T and Guestrin C. (2016). XGBoost: A Scalable Tree Boosting System. arXiv preprint arXiv: 1603.02754

### 4. 再排序

当召回、排序失效时，冷启动

[1]Andrew I. Schein, Alexandrin Popescul, Lyle H. Ungar, David M. Pennock. (2002). Methods and Metrics for Cold-Start Recommendations. Proceedings of the 25th Annual International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR 2002). New York City, New York: ACM. pp. 253–260.

### 5. 评估

线下预估和线上AB测试

[1]Beel, J.; Genzmehr, M.; Gipp, B. (2013). A Comparative Analysis of Offline and Online Evaluations and Discussion of Research Paper Recommender System Evaluation. Proceedings of the Workshop on Reproducibility and Replication in Recommender Systems Evaluation (RepSys) at the ACM Recommender System Conference (RecSys).
