# Ensemble

we can reduce the variance and improve the generalisation error by averaging over diﬀerent learning machines

## Bagging

Bootstrapping is to **resample** the initial data set we have into subsets

Bagging is to **average** the **regression** result or **vote/ take mode** the **classification** result on **bootstrapped** samples \(boosting uses the original data set\)

1. For categorization we get our diﬀerent machines to vote
2. For regression we can average the prediction of diﬀerent machines

## Boosting

In boosting we make a strong learner by using a **weighted** sum of weak learners, which do little better than chance and wont overfit much \(boosting uses the **original** data set\)

### Choosing weights:

**1. Adaboost** — a classic algorithm for **binary** problems, works well with **weak learners** instead of strong learners \(overfit\)

**2. Gradient boosting** — build a **strong learner** as a linear combination of weak learners and train a classiﬁer on the **residual errors** \(残差 the target minus the current prediction\)

It is easy to **over-fit**. we can use **early-stop** and **cross-validation** to prevent.

**3. XGBoost** — eﬃcient for gradient boosting on **large** data sets and the best method for **tabular** data

It uses a cleverly chosen **regularisation term** to favour simple trees and finds a clever way to approximately minimise error plus regulariser very fast

## Random Forests

In random forests we apply **bagging** and **average** much less correlated trees \(**decorrelated** trees\)

