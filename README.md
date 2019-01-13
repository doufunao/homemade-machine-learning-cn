# 自制机器学习
[homemade-machine-learning](https://github.com/trekhleb/homemade-machine-learning)

> 本项目包含了用 **Python** 实现流行的机器学习算法例子和他们背后的数学原理说明。每个例子包含交互的 **Jupyter Notebook** demo，你可以操作训练数据，算法配置，并且可以在你的播放器内立即看到结果、图表和预测值。本项目的大部分例子都基于吴恩达的《[机器学习课程](https://www.coursera.org/learn/machine-learning)》。

本项目的目的不在于使用第三方库仅用几行完成机器学习算法，而是从零开始，使用算法背后的数学进行编写。这也是为什么所有算法实现都被称为“自制”，而不是为了产品应用。

## 有监督学习 Supervised Learning

在有监督学习中，我们有一个训练数据集合作为输入，每个训练集合有一个标签或“真值”集合作为输出。然后，我们训练模型（机器学习算法参数）正确地映射（正确预测）输入和输出。最终目的是找到一组模型参数，可以成功的把新数据的输入映射（预测）到输出。

### 回归 Regression

我们在回归问题中进行真实值预测。一般我们试图在训练数据中绘制线/平面/n维平面。

用途举例：股价预测，销售分析，任意数字的依赖度等。

#### 🤖 线性回归 Linear Regression



### 分类器 Classification

#### 🤖 逻辑回归 Logistic Regression

- 📗 [数学 | 逻辑回归](homemade/logistic_regression) - 理论和延伸阅读链接
- ⚙️ [代码 | 逻辑回归](homemade/logistic_regression/logistic_regression.py) - 实现示例
- ▶️ [演示 | 逻辑回归 (线性边界)](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/logistic_regression/logistic_regression_with_linear_boundary_demo.ipynb) - 基于`花瓣长度`(`petal_length`)和`花瓣宽度`(`petal_width`)预测鸢尾花分类(`class`)
- ▶️ [演示 | 逻辑回归 (非线性边界)](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/logistic_regression/logistic_regression_with_non_linear_boundary_demo.ipynb) - 基于参数1(`param_1`)和参数2(`param_2`),预测芯片有效性(`validity`)
- ▶️ [演示 | 多元逻辑回归 | MNIST数据集](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/logistic_regression/multivariate_logistic_regression_demo.ipynb) - 识别`28x28`像素图片的手写数字
- ▶️ [演示 | 多元逻辑回归 | Fashion MNIST数据集](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/logistic_regression/multivariate_logistic_regression_fashion_demo.ipynb) - 识别`28x28`像素图片的衣服类型

## 无监督学习 Unsupervised Learning

### 聚类 Clustering

在聚类问题中我们利用未知的特性区分训练样本。算法本身会决定哪种特性用来区分。

_用途举例：市场划分， 社交网络分析， 组织计算集群，天文数据分析，图像压缩，等等._

#### 🤖 k-均值算法 K-means Algorithm

- 📗 [数学 | K-means 算法](homemade/k_means) - 理论和延伸阅读的链接
- ⚙️ [代码 | K-means 算法](homemade/k_means/k_means.py) - 实现示例
- ▶️ [演示 | K-means 算法](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/k_means/k_means_demo.ipynb) - 利用`花瓣长度`(`petal_length`)和`花瓣宽度`(`petal_width`)将鸢尾花分到多个类(clusters)

### 异常检测 Anomaly Detection

异常检测（也叫outliner deteciton）是识别出来与大多数数据有显著不同的样本，事件或观察样例。

用途举例：入侵检测，欺诈检测，系统良性检测，从数据集中取出异常数据等。

#### 🤖 应用高斯分布的异常检测 Anomaly Detection using Gaussian Distribution

*[[数学 | 应用高斯分布的异常检测](/homemade/anomaly_detection/README.md)]-理论和扩展阅读链接  

*[[代码 | 应用高斯分布的异常检测](/homemade/anomaly_detection/multilayer_perceptron.py)]-代码实例

*[[演示 | 异常检测](https://nbviewer.jupyter.org/github/trekhleb/homemade-machine-learning/blob/master/notebooks/anomaly_detection/anomaly_detection_gaussian_demo.ipynb)]-查找服务器操作参数（如延迟```latency```和阈值```threshold```）中的异常

### 神经网络 Neural Network (NN)

神经网络本身不是一个算法，而是一个框架，很多不同机器学习算法一起工作，处理复杂的输入。

用途举例：所有其他算法的替代算法，图像识别，语音识别，图像处理（应用特殊样式），语言翻译等。

#### 🤖 多层感知 Multilayer Perceptron (MLP)

* [[数学 | 多层感知器](/homemade/neural_network/README.md)] - 理论和扩展阅读链接



## 机器学习路线图



## 前提

#### 安装 Python

#### 安装依赖库

#### 启动本地 Jupyter

#### 启动远程 Jupyter



## 数据



## 贡献列表

| 章节                  | 译者 |
| --------------------- | ---- |
| Linear Regression     |      |
| Logistic Regression   |      |
| Anomaly Detection     |      |
| Anomaly Detection     |      |
| Multilayer Perceptron |      |

