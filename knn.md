# KNN

Classification: mode

Regression: mean

Regression KNN assigns value of unknown point based on average values of closest K neighbours in featurespace

It is important to choose the correct K. Too small, overfit. Too big, smooth too much.

Using **corss validation** to measure performance, K一般小于20

**Improving KNN**

距离越远，相似度越小，影响越小

Inverse weighting

$$
weight = k_1/(distance + k_2)
$$

subtraction weighting

$$
weight = max(0,k_1-distance)
$$

Gaussian weighting

$$
weight = exp(-distance^2/k_1^2)
$$

Advantanges: easy

Disadvantages: computationally expensive \(many examples generally means better accuracy\)

## K-D Trees

Query point - walk down the tree - find the nearest neighbour in the leaf - backtrack, and see if the next subtree needs checking - no need to check other subtrees - stop

K-D Tree does not scale well to high dimensions, it trends to end up searching most of the tree

