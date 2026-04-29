# 神经网络
神经网络和深度学习是有交集关系。 
## 神经网络的特征
1.信息表示是分布式的  
2.记忆和知识存储在单元之间的连接上  
3.通过改变连接的强度调整学习的大小  
## 激活函数
1. S型激活函数：sigmoid(logistic,tanh)  
![sigmoid](https://latex.codecogs.com/svg.image?\sigma(x)=\frac{1}{1+e^{-x}})、![tanh](https://latex.codecogs.com/svg.image?\tanh(x)=\frac{e^{x}-e^{-x}}{e^{x}+e^{-x}})  
2. 斜坡型激活函数  
（1）RELU ：  
优点【不会像sigmoid一样饱和、计算简单、一定程度上解决梯度下降的问题】  
缺点【小于0部分可能会永远不被激活、不是0均值，对梯度有影响】  
note:改进措施就是加一些min()或exp()这类的。  
（2）解决RELU死亡现象---->leaky RELU
（3）解决非0均值---->ELU
3. 复合激活函数  
（1） swish ： 是self-gated函数，其中的logistic函数值域（0，1），logistic值接近于1时值接近x（门开），反之亦然。  
（2） GELU(Gaussian error loss unit)  ： x*P(X<x)，和swish相似。

