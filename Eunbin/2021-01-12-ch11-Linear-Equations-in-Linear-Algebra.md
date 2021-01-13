---
layout: post
categories: Linear_Algebra
title: Ch11. Linear Equations in Linear Algebra
---


**A system of linear equations** : A collection of one or more linear equations   
**Solution Set** : The Set of all possible solutions of the linear system  
	→ Two linear systems are called **equivalent** if they have the same solution set.  


A system of linear equations has either
1. No Solution ( **INCONSISTENT** )
2. Exactly one Solution ( **CONSISTENT** )
3. Infinitely Many Solutions ( **CONSISTENT** )


## Matrix Notation
- 3 rows x 3 columns => Coefficient Matrix ( 3 $$\times$$ 3 ) : 계수 행렬
- 3 rows x 4 columns => Augmented Matrix ( 3 $$\times$$ 4  ) : 확대 행렬
	- 첨가 행렬은 계수 행렬과 상수항들의 행렬을 맞붙여 얻는 행렬

### Augmented Matrix
$$ A = \left[
\begin{matrix}
1 & 2 & 3 \\
4 & 7 & 4 \\
1 & 6 & 8 \\
\end{matrix}
\right] , B = \left[
\begin{matrix}
1 \\
4 \\
1 \\
\end{matrix}
\right]  $$
가 있을 때, Augmented Matrix 는
$$
\left[
\begin{matrix}
1 & 2 & 3  & 1\\
4 & 7 & 4 & 4 \\
1 & 6 & 8 & 1 \\
\end{matrix}
\right]  $$
이다.

### Elementary row operations
1. **Replacement**
2. **Interchange**
3. **Scaling**

Two matrices are **Row Equivalent** If there is a sequence of elementary row operations that transforms one matrix into the other.  
If the **augmented** matrices of the linear systems are **row equivalent**, then the two systems have the **same solution set**.  