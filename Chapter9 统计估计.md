# Chapter9 统计估计

到目前为止，已经讨论了随机变量和概率分布的各种性质。然而，在实践中，概率分布通常是未知的，只有样本可用。在本章中，给出了用于从样本中识别潜在概率分布的 *统计估计* 的概述。

## 9.1 统计估计基础

在样本中估计的量被称为 *估计量* 并且用“帽子”表示。例如，当通过样本平均值来估计概率分布的期望 <img src="http://latex.codecogs.com/gif.latex?\mu" style="border:none;"> 时，其估计量被表示为  

<img src="http://latex.codecogs.com/gif.latex?\hat{\mu}=\frac{1}{n}\sum_{i=1}^{n}x_i" style="border:none;"> 。  

估计量是样本 <img src="http://latex.codecogs.com/gif.latex?\left\{x_i\right\}_{i=1}^{n}" style="border:none;"> 的函数，因此是随机变量。另一方面，如果在估计量中插入特定值，则所获得的值被称为 *估计* 。  

用有限维参数 <img src="http://latex.codecogs.com/gif.latex?\theta" style="border:none;"> 描述的一组概率质量/密度函数被称为 *参数模型* ，并由 <img src="http://latex.codecogs.com/gif.latex?g(x;\theta)" style="border:none;"> 表示。在符号 <img src="http://latex.codecogs.com/gif.latex?g(x;\theta)" style="border:none;"> 中，分号之前的 <img src="http://latex.codecogs.com/gif.latex?x" style="border:none;"> 是随机变量，分号后的 <img src="http://latex.codecogs.com/gif.latex?\theta" style="border:none;"> 是参数。例如，对应于 <img src="http://latex.codecogs.com/gif.latex?d" style="border:none;"> -维正态分布的参数模型，  

<img src="http://latex.codecogs.com/gif.latex?g(x;\mu,\Sigma)=\frac{1}{(2\pi)^{\frac{d}{2}}\sqrt{\det(\Sigma)}}\exp(-\frac{1}{2}(x-\mu)^{T}\Sigma^{-1}(x-\mu))" style="border:none;"> ，  

其中有期望矢量 <img src="http://latex.codecogs.com/gif.latex?\mu" style="border:none;"> 和方差-协方差矩阵 <img src="http://latex.codecogs.com/gif.latex?\Sigma" style="border:none;"> 作为参数。  

通过识别参数模型中的参数来进行统计估计的方法被称为 *参数方法* ，而非参数方法则不使用参数模型或使用具有无限多个参数的参数模型。  

以下，假设样本 <img src="http://latex.codecogs.com/gif.latex?\mathfrak{D}=\left\{x_i\right\}_{i=1}^{n}" style="border:none;"> 为 <img src="http://latex.codecogs.com/gif.latex?i.i.d." style="border:none;"> 关于 <img src="http://latex.codecogs.com/gif.latex?f(x)" style="border:none;"> 的函数（详见 <img src="http://latex.codecogs.com/gif.latex?7.3" style="border:none;"> 节）。
