# SVM

The SVMs are typically used on **numerical** data, but can and have been adapted to text, sequences. Besides, they will often be the method of choice on **small** datasets. It relies on **distance** between data points.

The idea of SVMs is to find the **maximum-margin hyper-plane**. To increase the likelyhood of linear-separability, we often use a high-demensional mapping.

[svm](https://www.sohu.com/a/206572358_160850)

There are a number of strategies to make them multi-class, two frequent strategies

1. Train \|C\| one-versus-all classiﬁes and choose best

   某一类样本为一类，其他类别样本为一类，做K个SVM

2. Train \|C\|\(\|C\|−1\)/2 one-versus-one classiﬁes and vote for best

   任意两个样本之间做SVM，共K\(K-1\)/2个SVM

3. Using the class label as a feature

Positive semi-definite jernel function K\(x,y\)

## Advantanges & Disadvantanges

Advantanges:

1. Unique optimum 
2. It can over-fit, but well controlled
3. Limited amount of training data

Disadvantanges:

1. It requires very well written optimisers.
2. It can be very slow If the data set is large. The time complexity for training is O\(P^3\), P is the training patterns and it can be too slow if P&gt;&gt;1000

## Slack variables

Relax constrains by slack variables. \(松弛变量\)

## Kernel functions

Kernel functions are symmetric functions of two variables.

Strong restriction: positive semi-definite

When we use the kernel trick the time to compute the solution to the quadratic programming problem is **pN^3** where N is the number of training examples and p is the number of feature

