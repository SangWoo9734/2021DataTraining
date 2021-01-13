---
layout: post
categories: Linear_Algebra
title: Ch16. Linear Independence
---

### Linearly Independent
A set of vectors $${\mathbf{v_1}, \cdots, \mathbf{v_p}}$$ in $$\mathbb{R^n}$$ is said to be linearly independent, if the vector equation  
$$x\mathbf{v_1} + \cdots + x_p\mathbf{v_p} = 0$$  
Has only the trivial solution.   
trivial solution 만 있을 때, vector 앞에 있는 coefficient 가 다 0인 솔루션    
- 어떤 vector set 에 LD 를 따지는 것은, $$A\mathbf{x} = 0$$을 푸는 것과 동일함
- free variable이 한 개라도 존재하면, Nontrivial solution → 해가 무수히 존재

### Linearly Dependent
The set $${\mathbf{v_1}, \cdots, \mathbf{v_p}}$$ in $$\mathbb{R^n}$$ is said to be linearly dependent if there exist weights $$c_1, \cdots, c_p$$, **not all zero**, such that    
$$
c_1\mathbf{v_1} + \cdots + c_p\mathbf{v_p} = 0
$$   
$$c_1 \sim c_p$$ 중 최소 하나라도 nonzero  

### Linear Independence of Matrix Columns
$$
A = \left[ a_1, \cdots, a_n \right] \\
A\mathbf{x} = 0\\
x_1\mathbf{a_1} + x_2\mathbf{a_2} + \cdots + x_n\mathbf{a_n} = 0
$$  
The columns of a matrix $$A$$ are linearly independent if and only if the equations $$A\mathbf{x} = 0$$ has only the trivial solution.

#### Example. 
Determine if the columns of the following matrix are linearly independent.  
모든 row에 pivot position이 있고, free variable이 없음 → only trivial solution : Linearly independent


### Sets of One Vector
If a set contains only on vector, $$\mathbf{v}, then the set is linearly independent$$  
Only when $$\mathbf{v} \ne 0 \\
\because \mbox{ if } \mathbf{v} = 0, x_1\mathbf{v} = x_10 = 0$$  

### Sets of Two Vectors
하나의 vector가 다른 v의 곱으로 표현된다면 linearly Dependent  
A set $$\{\mathbf{v_1}, \mathbf{v_2}\}$$ is linearly dependent  
if at least one of the vectors is a multiple of the other $$\mathbf{v_1} = c\mathbf{v_2} \\ -\mathbf{v_1} + c\mathbf{v_2} = 0$$  
The set is linearly independent, if and only if neither of the vectors is a multiple of the other.    
$$x_1\mathbf{v_1} + x_2\mathbf{v_2} = 0$$ → $$\mathbf{v_1} = -(x_2 / x_1) \mathbf{v_2}$$ 는 맞지 않음 : 이 식 자체는 서로의 곱으로 표현되는데, 이는 즉 서로의 multiple 형태인 셈 → 불가능   

- A multiple of the other → linearly dependent
$$
\mathbf{v_1} = \left[ \begin{matrix}3\\1\\\end{matrix}\right]  \mathbf{v_2} = \left[ \begin{matrix}6\\2\\\end{matrix}\right] \\
\mathbf{v_2} = 2\mathbf{v_1} \\2\mathbf{v_1} - \mathbf{v_2} = 0
$$ 


- Neither → linearly independent
$$
\mathbf{v_1} = \left[ \begin{matrix}3\\3\\\end{matrix}\right]  \mathbf{v_2} = \left[ \begin{matrix}6\\2\\\end{matrix}\right] \\
x_1\mathbf{v_1} + x_2\mathbf{v_2}  = 0\\
\mathbf{x} = (0,0)  
$$   



#### 📖 Theorem 7. Characterisation of Linearly Dependent Sets
An indexed set $$S = \{\mathbf{v_1}, \cdots, \mathbf{v_p} \}$$ of two or more vectors Is linearly dependent   
	 (Non Trivial solution → 최소 하나의 벡터가 나머지 벡터의 linear combination으로 표현되는 경우)  
If and only if **at least** one of the vectors in $$S$$ is a linear combination of the others.  
In fact, if $$S$$ is linearly dependent and $$\mathbf{v_1} \ne 0$$, then some $$\mathbf{v_j}$$ (with j > 1) is a linear combination of the preceding vectors, $$\{v_1, \cdots, v_j-1\}$$   
$$j$$ : the largest subscript for which $$c_j \ne 0$$   
$$c_1\mathbf{v_1} + \cdots + c_p\mathbf{v_p} = 0$$   


### $${\mathbf{u}, \mathbf{v}, \mathbf{w}}$$ in $$\mathbb{R^3}$$
With $$\mathbf{u} \mbox{ and } \mathbf{v}$$ linearly independent (서로가 스칼라곱의 형태로 표현되지 않을 때 )  
$$\mathbf{w}$$ is in $$/mbox{span} \{\mathbf{u}, \mathbf{v}\}$$  
If and only if the set $${\mathbf{u}, \mathbf{v}, \mathbf{w}}$$ is linearly dependent.  
$$
\mathbf{w} = c\mathbf{u} + d\mathbf{v}, -\mathbf{w} + c\mathbf{u} + d\mathbf{v} = 0\\
\mathbf{u} \ne 0  \mathbf{u} \ne c\mathbf{v}
$$

#### 📖 Theorem 8.
If a set contains more vectors than there are entries in each vector, then the set is linearly dependent.  
When n rows p columns, $$p > n$$ must be a free variable!   
$$A\mathbf{x} = 0$$ has a nontrivial solution.

#### 📖 Theorem 8.
If a set contains the zero vector, then the set is linearly dependent.   
$$1\mathbf{v_1} + 0\mathbf{v_2} + \cdots + 0\mathbf{v_p} = 0$$