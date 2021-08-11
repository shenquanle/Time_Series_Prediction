# Time_Series_Prediction
ML/DL methods to predict time series
由于论文在投中，源码和数据暂不可公开，只能说下实验思想。

实验思想：

论文一：
对天文数据和传感器数据进行数据预处理，对各种不同类型的数据按照时间先后进行数据整合和对齐，根据时间间隔划分不同的时间序列，使用统计学模型（ARIMA、Prophet）、机器学习模型（MLP、XGBoost、LightGBM）、深度学习模型（LSTM、GRU、LSTM+XGBoost、GRU+XGBoost）分别建立预测模型，并进行预测效果的对比。

论文二：
在论文一的基础上，利用论文一中的实验结果作为论文对比实验的结果，在模型上基于RNN及其变体，引入时空双阶段注意力机制，通过特征自身历史信息的注意力机制、同一时刻特征之间的相互影响注意力机制，从而获取某时刻的一个更好的特征向量表示，从而保证预测值更好的拟合真实值。
