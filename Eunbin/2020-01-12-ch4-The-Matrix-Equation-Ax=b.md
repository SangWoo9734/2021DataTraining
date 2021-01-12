---
categories: Linear_Algebra
title: Ch04. The Matrix Equation Ax=b
---

### $$A\mathbf{x}$$ : Product of A and x
The linear combination of the columns of $$A$$ using the corresponding entries in $$\mathbf{X} \mbox{ as weights}$$ → x 벡터 엔트리가 가중치


### 📖 Theorem 3.
$$A$$ is $$m \times n$$ matrix, with columns $$a_1, \cdots, a_n   \mathbf{b} \mbox{ is in }\mathbb{R}^m$$
1. Matrix Equation : $$A\mathbf{x} = \mathbf{b}$$
2. Vector Equation : $$ x_1\mathbf{a_1} + x_2\mathbf{a_2} + \cdots + x_p\mathbf{a_p} = \mathbb{b}$$
3. Augmented Matrix  : $$\left[ \mathbf{a_1}, \mathbf{a_2}, \cdots, \mathbf{a_n} \mathbf{b}\right]$$

Have the same solution set!


### 📖 Theorem 4.
The followings are all true of all false:
1. For each b in R^m, Ax = b  has a solution
2. Each b in R^m is a linear combination of the columns of A
3. The columns of A spanR^m
4. A has a pivot position in every row

### 📖 Theorem 5.
If A is an m x n matrix, u and v are vectors in R^m,  And c is a scalar, then;    
A(u + v) = Au + Av;  
A(cu) = c(Au)