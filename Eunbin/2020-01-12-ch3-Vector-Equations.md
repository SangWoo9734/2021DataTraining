---
categories: Linear_Algebra
title: Ch03. Vector Equations
---

Vectors in $$\mathbb{R}^2$$ → 실수 2차원 공간   
$$\mathbf{u} = \left[\begin{matrix}3 \\ -1 \\\end{matrix}\right], \mathbf{v} = \left[\begin{matrix}0.2 \\ 0.3 \\\end{matrix}\right], \mathbf{u} = \left[\begin{matrix}w_1 \\ w_2 \\\end{matrix}\right]$$  
$$\vec{u} = (3, -1), \vec{v} = (0.2, 0.3), \vec{w} = (w_1, w_2)$$   

$$(w_1, w_2) \ne \left[ w_1, w_2\right]$$

### Scalar Multiplication
백터 네 모든 값에 스칼라 값을 곱해준다  
$$c = 5, \mathbf{u} =  \left[\begin{matrix}3 \\ -1 \\\end{matrix}\right]$$ 일 때,  
$$
c\mathbf{u} = 5 \left[\begin{matrix}3 \\ -1 \\\end{matrix}\right] =  \left[\begin{matrix}5\cdot3 \\ 5\cdot(-1) \\\end{matrix}\right] =  \left[\begin{matrix}15 \\ -5 \\\end{matrix}\right]
$$  


### Vectors in $$\mathbb{R}^n$$
$$
c\mathbf{u} = \left[\begin{matrix}u_1 \\ u_2 \\ \cdots \\ u_n\end{matrix}\right]   \\
\mathbf{u} = (u_1, u_2, \cdots, u_n)
$$   

### Algebraic Properties of $$\mathbb{R}^n$$
**$$\mathbf{u, v, w} \mbox{ are } \mathbb{R}^n \mbox{ and } c d \mbox{ are scalar}$$**
1. u + v = v + u
2. (u + v) + w = u + (v + w)
3. u + 0 = 0 + u = u
4. u + (-u) = -u + u = 0
5. c(u + v) = cu + cv
6. (c + d)u = cu + du
7. c(du) = (cd)u
8. 1u = u

### Linear Combinations
**Linear combination of $$\mathbf{v_1, v_2, \cdots, v_p} \mbox{ is } \mathbb{R}^n     
\mbox{with weights } c_1, c_2, \cdots, c_p \mbox{ is scalar}$$**    

y = $$ c_1\mathbf{v_1} + c_2\mathbf{v_2} + \cdots + c_p\mathbf{v_p}$$  


A vector equation   
$$x_1\mathbf{a_1}+x_2\mathbf{a_2}+\cdots+x_n\mathbf{a_n} = \mathbf{b}$$  
has the **same solution** set as the linear system whose **augmented matrix** is    
$$\left[\mathbf{a_1} \mathbf{a_2} \cdots \mathbf{a_n} \mathbf{b}\right]$$   

→ 각 벡터를 집어넣은 Augmented Matrix 와 동일한 해를 지닌다.

### Span{$$\mathbf{v}$$}
is the collection of all vectors that can be written in the form  
 $$ c_1\mathbf{v_1} + c_2\mathbf{v_2} + \cdots + c_p\mathbf{v_p}$$  

