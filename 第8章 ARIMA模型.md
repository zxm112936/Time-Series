# 第8章 ARIMA模型

_____

+ ARIMA是另一种时间序列预测的方法。

+ 指数平滑模型 （exponential smoothing) 和 ARIMA 模型是应用最为广泛的两只时间序列预测方法。
+ 指数平滑模型针对于数据中的趋势（trend）和季节性（seasonality）不同， ARIMA模型描绘数据的自回归性（autocorrelations）。

在引入ARIMA模型前，我们需要先讨论平稳性（stationarity）和差分时间序列（differencing time series）。

## 8.1 平稳性和差分

___

+ 平稳的时间序列的性质不随观测时间的变化而变化

​       性质指：

​       $E（X_{t}）=\mu， Var（X_{t}）=\sigma^{2}, Cov(X_{t},X_{t+k})=\gamma_{k}$

+ ==所以具有趋势或季节性的时间序列不是平稳时间序列==

+ 白噪音序列（white noise series） 是平稳的

  $E(\epsilon_{t}) = 0, Var(\epsilon_{t}) = \sigma^{2}_{\epsilon}, Cov(\epsilon_{t}, \epsilon_{t+k})= 0$

+ ==如果一个循环变化的时间序列没有趋势和季节性$\Rightarrow$那么它仍然是平稳的。== 

  理由：因为这些循环变化并没有一个固定的周期，因此在进行观测之前我们无法知道循环变化的峰值和谷值会出现在哪个位置。

  	第二条+第四条 

​	==时间序列没有趋势和季节性$\Leftrightarrow$时间序列平稳==

+ 平稳的时间序列从长期来看不存在可预测的特征

+ 

![1min CORV_changed_May](C:\Users\45169\Desktop\Summer project data\RV picture\CoRV\1min CORV_changed_May.png)











