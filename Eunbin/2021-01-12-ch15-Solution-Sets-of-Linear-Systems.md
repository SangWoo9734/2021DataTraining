---
layout: post
categories: Linear_Algebra
title: Ch15. Solution Sets of Linear Systems
---


### Homogeneous Linear Systems
**Trivial solution**   
$$A\mathbf{x} = 0$$ (→ 제로 백터 ) always has at least one solution $$\mathbf{x} = 0$$   

**NonTrivial solution**   
If and only if the equation has at least one free variable → 유일하거나 무한히 많을 때  

#### 📖 Theorem2. Existence and Uniqueness Theorem
If a linear system is consistent, then the solution set contains either (i) a **unique solution**, when there are **no free variables**, or (ii) **infinitely many solutions**, when there is **at least one free variable**


$$A\mathbf{x} = 0$$    the solution set can always be expressed as 
$$
Span\{\mathbf{v_1}, \mathbf{v_2}, \cdots, \mathbf{v_p}\}
$$  
Trivial Solution :  $$Span\{0\} $$ → v를 0벡터로 표현

### NonHomogeneous Linear Systems
$$A\mathbf{x} = \mathbf{b}$$ →b is nonzero vector  

#### 📖 Theorem6. 
Suppose    
$$A\mathbf{x} = \mathbf{b}$$ is consistent (→ 해가 최소 1개 이상일 때)  And let $$\mathbf{p}$$ be a solution ( → p 벡터가 솔루션이라 가정하며 )  
Then the solution set of $$A\mathbf{x} = \mathbf{b}$$ is the set of all vectors of the form   
$$\mathbf{w} = \mathbf{p} + \mathbf{v_h}$$ where $$/mathbf{v_h}$$ is any solution of the homogeneous equation $$A\mathbf{x} = \mathbf{0}$$