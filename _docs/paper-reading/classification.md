---
title: classification of flow and nonflow
category: Paper Reading
order: 1
---

- [1. INTRODUCTION](#1-introduction)
- [2. MACHINE LEARNING MODELS](#2-machine-learning-models)
- [3. DATA PREPARATION](#3-data-preparation)
- [4. RESULTS](#4-results)

## 1. INTRODUCTION

## 2. MACHINE LEARNING MODELS

> A. Principal Component Analysis
>+ more data prefer "machine learning", difficult ro visualize and understand
>+ PCA: 对数据降维，只保留原始数据中最重要的信息
  换坐标系来降低principal components之间的耦合
>+ 给dataset：$X_{n\times m}=[x_1,…,x_m]$
  n个sample，每个sample是m维向量(有m个feature)
>1. centralize:
    $z_i=x_i-\mu_i$
    其中$\mu=\frac{1}{n}\sum\limits_{i=1}^{n}x_i$,是n个sample element-wise的平均值
>2. covariance matrix 协方差矩阵
   $\Sigma=\frac{1}{n}\sum\limits_{i=1}^{n}z_iz_i^{T}=\frac{1}{n}Z\cdot Z^{T}$
>3. 计算convariance matrix的本征值
   <font color=RoyalBlue>? 目的是把$\Sigma$对角化，来消除不同坐标之间的耦合</font>
   $\Sigma u=\lambda u$
   可以把对应比较大本征值的向量作为新的基矢量
   <font color="RoyalBlue">? 特征值一定都是正的吗
   ? 这个PCA跟机器学习有什么关系</font>


> B. Point Cloud Networks
>跟CNN的主要区别：
>1. point change symmetry
    <font color="RoyalBlue"> ? momentem 作为input feature有point exchange symmetry吗</font>
>2. 平移旋转不变性
>- global maximum pooling
>- T-net

## 3. DATA PREPARATION
> A. Two particle correlation
><font color=RoyalBlue>? 这里两个$N_{trig}$数值一样<br>? 量纲对吗</font>

![image.png](https://s2.loli.net/2022/07/09/e8sKtQqIjazXC4l.png)

> B. Particle cloud
>输入是所有粒子的三维动量

## 4. RESULTS
> A. Classification via two particle correlation
>- small system 和 large system 的 model 不能混起来用
>- <font color=RoyalBlue>? 这里的input还是two particle correlation吗</font>

> B. Event by event classification
><font color=RoyalBlue>? 这里的input是三维动量</font>
