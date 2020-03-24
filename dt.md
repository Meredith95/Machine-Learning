# DT

**Interpretability** 可解释性

DTs are particularly good for handling messy data, **categorical data**, **missing data**, **mixture of data types**, **large data sets**, **multiclass**.

Decision trees builds a **binary tree** to partition the data into the leaves of the tree. It can also be used for **regression** problems, with the approximate function \(**CART**\).

## Algorithms

ID3, information gain. 越大越好

C4.5, gain ratio. 越大越好

CART, gini impurity. 越小越好

前两种方法都用到了entropy，log计算会导致运算速度变慢。

## Leaf Purity

1. Gini 
2. Entropy
3. Variance \(for regression\) 

**Advantanges & Disadvantages**

Advantanges:

1. Useful for exploring dataset by visualising the tree /  DTs make the reasoning process explicit
2. Flexiable with numerical and categorical data. 

Disadvantages:

1. DTs depend strongly on the **early decisions** and so vary a lot for slightly diﬀerent data sets, which result in **high variance**. 
2. DTs are **correlated**, which boosting could do better
3. DTs trend to **overfit** and **generalise poorly** to new data set
4. Might not effectively scale to **large** numbers of classes 

