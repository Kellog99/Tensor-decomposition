# Tensor-decomposition

Description:
Welcome to the "Deep Learning and Singular Value Decomposition (SVD)" repository on GitHub! In this repository, we explore the fundamental concepts behind Singular Value Decomposition and its invaluable role in enhancing deep learning algorithms.

### What is Singular Value Decomposition (SVD)?
Singular Value Decomposition is a powerful mathematical technique used for dimensionality reduction, data compression, and feature extraction. It is especially relevant in the context of deep learning, where large datasets and complex neural networks are common.

### How SVD Works:
SVD decomposes a matrix into three separate matrices, $U, \Sigma$ and $V^T$, where:

- $U$: Represents the left singular vectors and encodes the input data's structure.
- $\Sigma$: Is a diagonal matrix containing the singular values, which quantify the importance of each singular vector.
- $V^T$: Represents the right singular vectors and encodes the relationships between features or patterns.

By approximating the original matrix with a truncated version of these three matrices, we can reduce the data's dimensionality while preserving the most important information. 

Moreover, it is always possible to control the error generated by the compression with the following theorem


**Theorem**

Let $A\in \mathbb{R}^{m\times n}$ be a matrix of rank $r$ with the following SVD $A= U\Sigma V^{T}$ with $\Sigma=diag(\sigma_1,\cdots,\sigma_r)$ and $\sigma_i\geq\sigma_{i+1}>0$. Then 
    $$\min_{rank(B) \leq k}\|A-B\|=\left\|A-\sum_{i=1}^k\sigma_{i}u_i\otimes v_i\right\| = \sqrt{\sum_{i=k+1}^r\sigma_i^2}$$
    Where the norm is the Frobenius norm and $k\in \{1,\cdots, r\}$

