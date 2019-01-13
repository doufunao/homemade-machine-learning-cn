# K-Means 算法

## Jupyter 演示

▶️ [演示 | K-means 算法](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/k_means/k_means_demo.ipynb) - 使用`花瓣长度`(`petal_length`)和`花瓣宽度`(`petal_width`)将鸢尾花分到多个类(clusters)

## 定义

**K-means 聚类** 旨在将n个观测值分到_K_个类中，其中每一个观测值分到离它最近的类作为初步分类结果。

聚类分析的结果如下图所示，不同颜色的方块被分到三个类(cluster)中。

![Clustering](https://upload.wikimedia.org/wikipedia/commons/c/c8/Cluster-2.svg)

## 描述

给一个观测值的训练集:

![Training set](../../images/k_means/training-set.svg)

![x-i](../../images/k_means/x-i.svg)

每个观测值是一个_d_维的实数向量,k-means聚类旨在将_m_个观测值分到_K_ (_≤ m_)个类中:

![Clusters](../../images/k_means/clasters.svg)

... 以便于使每个类中方块总数量最小(即方差值).

下图中你可以看到一个例子，4个随机初始化的类中心点和集群收敛结果:

![Clustering](http://shabal.in/visuals/kmeans/random.gif)

[图片来源](http://shabal.in/visuals/kmeans/6.html)

另一个k-means聚类收敛的形象演示:

![Clustering](https://upload.wikimedia.org/wikipedia/commons/e/ea/K-means_convergence.gif)

## 损失函数 (Distortion)

![c-i](../../images/k_means/c-i.svg) - 样本 _x<sup>(i)</sup>_ 当前被分配到序号为 _(1, 2, ..., K)_ 的类的中心点.

![mu-k](../../images/k_means/mu-k.svg) - 第 _k_ 类的中心点 (![mu-k-2](../../images/k_means/mu-k-2.svg)) 并且 ![k](../../images/k_means/k.svg).

![mu-c-i](../../images/k_means/mu-c-i.svg) - 样本 _x<sup>(i)</sup>_ 上次被分配到的类的中心点.

举个例子:

![Cluster example](../../images/k_means/cluster-example.svg)

在这个例子中，优化目标如下所示：

![Cost Function](../../images/k_means/cost-function.svg)

![Clustering](https://upload.wikimedia.org/wikipedia/commons/d/d1/KMeans-density-data.svg)

## 算法

随机初始化 _K_ 个类的中心点 (随机计算 _K_ 个训练样本并且把 _K_ 个类的中心点分配给这几个样本).

![Centroids](../../images/k_means/centroids.svg)

![k-means-algorithm](../../images/k_means/k-means-algorithm.svg)

## 引用

- [Machine Learning on Coursera](https://www.coursera.org/learn/machine-learning)
- [K-means on Wikipedia](https://en.wikipedia.org/wiki/K-means_clustering)
