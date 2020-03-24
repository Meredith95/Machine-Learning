# Introduction

## Bias - Variance Dilemma

The dilemma means that a simple machine is likely to have a high bias but low variance, while a complex machine will have a low bias but a high variance.

**Bias**: generalisation performance of the mean machine.

Larger bias, simpler machine.

预测值和真实值之间的差异，即模型的精准度。

**Variance**: variation in the prediction of the machine as we change the data set.

Larger variance, more complex machine.

预测值和预测期望之间的误差，即模型的稳定性。

## The complexity of machine

**Generalisation** \(泛化\) : how well do we do on unseen data as supposed to the training data.

**Overfitting**: fitting the trainging data well at the cost of getting porer generalisation performance.

训练误差低，但测试误差高

**Underfitting**:

训练误差和测试误差都高

## Regularisation term

1. Punish large weights, which result in large changes in the prediction when the corresponding feature changes. 
2. Reduce variance and reduce the sensitivity of the model to the data. 

## Dimensionality Reduction

1. Less features \(Feature selection\)
2. Project data onto a lower dimensional sub-space \(PCA\)
3. cluster to find examplars and recode data \(RBF\)

### Imbalance

