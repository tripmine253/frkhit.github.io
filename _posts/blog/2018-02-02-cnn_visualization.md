---
layout: post
title: CNN可视化研究
category: 技术
tags: 
    - CNN
keywords: 
description: 
---

# CNN可视化研究

## 1.AlexNe可视化

### 1.1 Hinton原文
- 可视化第一层，输入224X224X3,卷积核96X11X11, 所以得到(96, 11, 11, 3)，共96张rgb图片
- gpu1上的图片，大多与颜色不相关: 高频率的灰度图
- gpu2上的图片，对应特定的颜色: 低频率的彩色图
- 总结: 其实是可视化权值

### 1.2 其他论文
[来源](http://blog.csdn.net/kangroger/article/details/55681374)

- 猫图输入,研究各层经过某些过滤器后得到的激活图
- 结论: 激活图看起来相对点状且密集,随着训练进行，激活图变得稀疏，激活值出现在某一区域
- 激活图是稀疏的（大部分值为零）且在某些固定位置激活



