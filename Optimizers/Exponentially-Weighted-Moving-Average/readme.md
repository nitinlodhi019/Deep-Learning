# **EWMA**

In deep learning, "EWMA" stands for "Exponentially Weighted Moving Average," which is a statistical technique used to calculate a running average by giving more weight to recent data points, effectively capturing trends in time-series data and often employed in optimizer algorithms like Adam to adjust learning rates based on recent updates, making them more responsive to changes in the loss function. 

**Key points about EWMA:**

1. *Prioritizes recent data:*
Unlike a simple moving average, EWMA assigns exponentially decreasing weights to older data points, allowing it to better track recent trends.
 
2. *Parameter "alpha":*
The degree of emphasis on recent data is controlled by a parameter called "alpha" - a value between 0 and 1, where a higher alpha means more weight is given to recent observations. 

**Application in optimizers:**

In deep learning optimizers like Adam, EWMA is used to calculate the exponentially weighted average of the gradient and its squared values, which helps to smooth out fluctuations and prevent the learning process from getting stuck in local minima. 
