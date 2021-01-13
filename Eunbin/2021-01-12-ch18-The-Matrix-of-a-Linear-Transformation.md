---
layout: post
categories: Linear_Algebra
title: Ch18. The Matrix of a Linear Transformation
---

#### 📖 Theorem 10.
Let $$T : \mathbb{R^n} \to \mathbb{R^m}$$ be a linear transformation. Then there exists a unique matrix A such that  
$$
T(\mathbf{x}) = A\mathbf{x} \mbox{ for all }\mathbf{x} \mbox{ in }\mathbb{R^n}
$$  
In fact, $$A$$ is the $$m \times n$$ matrix whose j-th column is the vector $$T(e_j)$$, where $$e_j$$ is the j-th column of the identity matrix in $$\mathbb{R^n}$$:  
$$A = \left[ T(e_1) \cdots T(e_n) \right]$$  
Standard matrix for the linear transformation T

### Onto
A mapping $$T: \mathbb{R^n} \to \mathbb{R^m}$$ is said to be **onto $$\mathbb{R^m}$$** if each $$\mathbf{b}$$ in $$\mathbb{R^m}$$ is the image of at least one $$\mathbf{x}$$ in $$\mathbb{R^n}$$

### One-to-one
A mapping  $$T: \mathbb{R^n} \to \mathbb{R^m}$$ is said to be **one-to-one** if each $$\mathbf{b}$$ in $$\mathbb{R^m}$$ is the image of at most one $$\mathbf{x}$$ in $$\mathbb{R^n}$$  
- 여러 개의 벡터에서 같은 이미지로 도달할 때 : one-to-one이 아님  
- 1대1 대응 : one-to-one


#### 📖 Theorem 11.
Let $$T: \mathbb{R^n} \to \mathbb{R^m}$$ be a linear transformation.  
Then $$T$$ is **one-to-one** if and only if the equation $$T(\mathbf{x}) = 0$$  has only trivial solution.  
$$
T(0) = T(0\mathbf{0}) = 0T(\mathbf{0})\\
T(\mathbf{u} = \mathbf{b}  T(\mathbf{v} = b)\\
T(\mathbf{u} - \mathbf{v}) = T(\mathbf{u}) - T(\mathbf{v}) = 0\\
\mathbf{u} - \mathbf{v} \ne 0
$$  
$$T(\mathbf{x}) = 0$$ has more than one solution

#### 📖 Theorem 12.
Let $$T: \mathbb{R^n} \to \mathbb{R^m}$$ be a linear transformation and let $$A$$ be the standard matrix for $$T$$.    
Then $$T$$ maps **$$\mathbb{R^n} \mbox{onto} \mathbb{R^m}$$** if and only if the **columns of $$A$$ span $$\mathbb{R^m}$$**     
$$T$$ is **one-to-one** if and only if the columns of $$A$$ are **linearly independent**.   
	one-to-one → only trivial → independent 