---
layout: post
title: "中产的极限"
author: "cong li"
date: 2018-12-06 12:12:45
header-style: text
tags: 
- 商业分析
- 资源分配
- 收入NPV 
---
**问题：中产30-60岁，累计收入在30岁时点的贴现值？**

假设：IRR=5%，不计通胀（薪酬有抗通胀性）

  * 策略一：30岁，30万/年. 匀速增到45岁，70万/年. 45-55岁，70万/年. 55-60, 50万/年.
  * 策略二：30岁，30万/年. 31岁，70万/年，保持到35岁。36岁120万/年，保持到40岁。40-45岁，50万/年.
  * 策略三：30岁，30万/年. 匀速增到45岁，150万/年。45-60岁，100万/年.

NPV分别是：816万，831万，1353万.

```r
#R codes
npv=function(a,i){
for(j in 1:length(a)){a[j]=a[j]*(1+i)^(-j)}
return(a)
}
plan_1=c(seq(from=30,to=70,length=15),rep(70,10),rep(50,5))
plan_2=c(30,rep(70,5),rep(120,5),rep(50,5))
plan_3=c(seq(from=30,to=150,length=15),rep(100,15))
sum(npv(plan_1))
sum(npv(plan_2))
sum(npv(plan_3))
```

