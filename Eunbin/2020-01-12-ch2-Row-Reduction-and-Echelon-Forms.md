---
categories: Linear_Algebra
title: Ch02. Row Reduction and Echelon Forms
---

**A leading Entry of row** : the LEFTMOST nonzero entry.   
### Echelon Form
1. All nonzero rows are above any rows of all zeros
2. Each leading entry of a row is in column to the right of the leading entry of the row above it
3. The leading entry in each nonzero row is 1
4. Each leading 1 is the only nonzero entry in its column


$$ 
1 → \left[
\begin{matrix}
\bullet & * & * & * \\
0 & \bullet & * & * \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{matrix}
\right]        
  2 → \left[
\begin{matrix}
\bullet & * & * & * \\
0 & \bullet & * & * \\
0 & 0 & \bullet & * \\
0 & 0 & 0 & \bullet \\
\end{matrix}
\right] 
$$


#### 📖 Theorem 1. Uniqueness of the Reduced Echelon Form
Each matrix is row equivalent to one and only one reduced echelon matrix

### Row Reduction Algorithm
1. Begin with the leftmost nonzero column
2. Select a nonzero entry in the pivot column as a pivot. If necessary, Interchange rows to move this entry into the pivot position.
3. Row replacement to create zeros in all positions below the pivot.
4. Apply steps 1-3 to the sub matrix that remain. The combination of steps 1-4 is called forward phase echelon form
5. Beginning with the rightmost polio and working upward and to the left, created zeros above each pivot. If a pivot is not 1, make it 1 by a scaling operation.  
	- Called backward phase reduced echelon form

### Solution of linear systems
$$ 
\left[
\begin{matrix}
1 & 0 & -5 & 1 \\
0 & 1 & 1 & 4 \\
0 & 0 & 0 & 0 \\
\end{matrix}
\right]   
$$   
일 때,  
$$
x_1 - 5x_3 = 1 \\
x_2 + x_3 = 4 \\
0 = 0 \\
\left[
\begin{matrix}
6 \\3 \\1 \\
\end{matrix}
\right]
\left[
\begin{matrix}
-9 \\
6 \\
-2 \\
\end{matrix}
\right]  \cdots
$$   
해가 무한대가 되며,  General Solution 은 아래와 같다.  
$$
\begin{cases}
x_1 = 1 + 5x_3 & \mbox{basic / leading  variables} \\
x_2 = 4 - x_3 & \mbox{basic / leading variables} \\
x_3 \mbox{ is free} & \mbox{free variable}
\end{cases}
$$  

#### 📖 Theorem 2. Existence and Uniqueness Theorem
A linear system is consistent if and only if the rightmost column of the augmented matrix is not a pivot column - that is, if and only if and echelon form of the augmented matrix has no row of the forms.    
$$\left[ \begin{matrix} 0 & \cdots &  0 & b \end{matrix} \right]$$ with $$b$$ is nonzero.    
If a linear system is consistent, then the solution set contains either (i) a unique solution, when there are no free variables, or (ii) infinitely many solutions, when there is at least one free variables.  