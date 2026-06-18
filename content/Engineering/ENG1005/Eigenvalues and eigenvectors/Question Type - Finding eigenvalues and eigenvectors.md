> [!NOTE] Finding [[Eigenvalue(s)]] and [[Eigenvector(s)]]
> We want to find a scalar $\lambda$ and a non-zero vector $\mathbf{v}$ such that:
>
> $$
> A\mathbf{v}=\lambda \mathbf{v}
> $$
>
> Rearranging:
>
> $$
> \begin{align}
> A\mathbf{v}-\lambda \mathbf{v}&=0\\
> A\mathbf{v}-\lambda I\mathbf{v}&=0\\
> (A-\lambda I)\mathbf{v}&=0
> \end{align}
> $$
>
> For a non-trivial solution $\mathbf{v}\neq \mathbf{0}$ to exist:
>
> - The matrix $(A-\lambda I)$ must **not be invertible**
> - Therefore:
>
> $$
> \det(A-\lambda I)=0
> $$
>
> This is called [[the characteristic equation]], which equates the determinant of the [[characteristic equation]], that is, the [[characteristic polynomial]] to 0, and solving it gives the eigenvalues $\lambda$.
>
> Then substitute each $\lambda$ back into $(A-\lambda I)\mathbf{v}=0$ to find the corresponding eigenvectors.

We can also determine the [[number of eigenvalues and eigenvectors of matrix]].

# Example 1: Repeating eigenvalues

Find the eigenvalues and eigenvectors of  $A=\begin{pmatrix}  1 & \tfrac{1}{2} \\  0 & 1  \end{pmatrix}$.

**Step 1: Find eigenvalues using the characteristic equation**

$$
\begin{align}
\det(A-\lambda I)&=0 \\
\det\begin{pmatrix}
1-\lambda & \tfrac{1}{2} \\
0 & 1-\lambda
\end{pmatrix}&=0 \\
(1-\lambda)^2&=0
\end{align}
$$

Hence, $\lambda=1$ (repeated eigenvalue)

**Step 2: Find eigenvectors by solving $(A-\lambda I)\mathbf{v}=0$**

$$
\begin{align}
(A-\lambda I)\mathbf{v}&=0 \\
\begin{pmatrix}
1-1 & \tfrac{1}{2} \\
0 & 1-1
\end{pmatrix}
\begin{pmatrix}
v_1\\
v_2
\end{pmatrix}&=
\begin{pmatrix}
0\\
0
\end{pmatrix} \\
\begin{pmatrix}
0 & \tfrac{1}{2} \\
0 & 0
\end{pmatrix}
\begin{pmatrix}
v_1\\
v_2
\end{pmatrix}&=
\begin{pmatrix}
0\\
0
\end{pmatrix}
\end{align}
$$

**Step 3: Solve the resulting system**
We know that the system must have at least one free parameter because otherwise there would be the unique solution $\mathbf{v}=\mathbf{0}$.

$$
\begin{align}
\tfrac{1}{2}v_2&=0 \\
v_2&=0
\end{align}
$$

Let $v_1=t$ (free parameter), then $\mathbf{v}=t\begin{pmatrix}1\\0\end{pmatrix}$

- Eigenvalue: $\lambda=1$ (repeated)
- Eigenvectors: $\mathbf{v}=t\begin{pmatrix}1\\0\end{pmatrix},\ t\in\mathbb{R},\ t\neq0$

# Example 2: two distinct eigenvalues

Find the eigenvalues and eigenvectors of

$$
A=\begin{pmatrix}
4 & -2\\
5 & -3
\end{pmatrix}
$$

**Step 1: Find eigenvalues using the characteristic equation**

$$
\begin{align}
\det(A-\lambda I)&=0 \\
\det\begin{pmatrix}
4-\lambda & -2\\
5 & -3-\lambda
\end{pmatrix}&=0 \\
(4-\lambda)(-3-\lambda)+10&=0 \\
\lambda^2-\lambda-2&=0
\end{align}
$$

$$
\begin{align}
\lambda&=\frac{1\pm\sqrt{1+8}}{2}=\frac{1\pm3}{2}
\end{align}
$$

Hence, $\lambda=2,\ -1$

**Step 2: For each eigenvalue, solve $(A-\lambda I)\mathbf{v}=0$**

**Case 1: $\lambda=2$**

$$
\begin{align}
(A-2I)\mathbf{v}&=0 \\
\begin{pmatrix}
2 & -2\\
5 & -5
\end{pmatrix}
\begin{pmatrix}
v_1\\
v_2
\end{pmatrix}&=
\begin{pmatrix}
0\\
0
\end{pmatrix} \\
2v_1-2v_2&=0
\end{align}
$$

Let $v_2=t$, then $v_1=t$

$$
\mathbf{v}=t\begin{pmatrix}1\\1\end{pmatrix},\ t\in\mathbb{R},\ t\neq0
$$

**Case 2: $\lambda=-1$**

$$
\begin{align}
(A+I)\mathbf{v}&=0 \\
\begin{pmatrix}
5 & -2\\
5 & -2
\end{pmatrix}
\begin{pmatrix}
v_1\\
v_2
\end{pmatrix}&=
\begin{pmatrix}
0\\
0
\end{pmatrix} \\
5v_1-2v_2&=0
\end{align}
$$

Let $v_2=t$, then $v_1=\tfrac{2}{5}t$

$$
\mathbf{v}=t\begin{pmatrix}\tfrac{2}{5}\\1\end{pmatrix},\ t\in\mathbb{R},\ t\neq0
$$

- $\lambda=2$, $\mathbf{v}=t\begin{pmatrix}1\\1\end{pmatrix}$
- $\lambda=-1$, $\mathbf{v}=t\begin{pmatrix}\tfrac{2}{5}\\1\end{pmatrix}$

# Example 3: 3×3 matrix

Find the eigenvalues and eigenvectors of

$$
A=\begin{pmatrix}
0 & 1 & 1\\
1 & 0 & 1\\
0 & 0 & 2
\end{pmatrix}
$$

**Step 1: Find eigenvalues using the characteristic equation**

$$
\begin{align}
\det(A-\lambda I)&=0 \\ \\
\det\begin{pmatrix}
-\lambda&1&1\\
1&-\lambda&1\\
0&0&2-\lambda
\end{pmatrix}&=0 \\ \\
(-\lambda)(-\lambda)(2-\lambda)-1(2-\lambda)&=0 \\
-\lambda^3+2\lambda^2+\lambda-2&=0
\end{align}
$$

$$
\begin{align}
\lambda^3-2\lambda^2-\lambda+2&=0 \\
(\lambda-1)(\lambda^2-\lambda-2)&=0
\end{align}
$$

$$
\begin{align}
\lambda&=1,\quad \lambda=\frac{1\pm3}{2}
\end{align}
$$

Hence,

$$
\lambda=1,\ 2,\ -1
$$

**Step 2: For each eigenvalue, solve $(A-\lambda I)\mathbf{v}=0$**

## Case 1: $\lambda=1$

$$
\begin{align}  
(A-I)\mathbf{v}&=0\\  \\
\begin{pmatrix}  
-1&1&1\\  
1&-1&1\\  
0&0&1  
\end{pmatrix}  
\begin{pmatrix}  
v_1\\v_2\\v_3  
\end{pmatrix}  
&=  
\begin{pmatrix}  
0\\0\\0  
\end{pmatrix}  
\end{align}  
$$

Augmented matrix:

$$
\left[  
\begin{array}{ccc|c}  
-1&1&1&0\\  
1&-1&1&0\\  
0&0&1&0  
\end{array}  
\right]  
$$

Gaussian elimination:

$$
\begin{align}  
R_2&\to R_2+R_1  
\end{align}  
$$

$$
\left[  
\begin{array}{ccc|c}  
-1&1&1&0\\  
0&0&2&0\\  
0&0&1&0  
\end{array}  
\right]  
$$

$$
\begin{align}  
R_3&\to R_3-\frac12R_2  
\end{align}  
$$

$$
\left[  
\begin{array}{ccc|c}  
-1&1&1&0\\  
0&0&2&0\\  
0&0&0&0  
\end{array}  
\right]  
$$

Thus:

$$
\begin{align}  
2v_3&=0\\  
v_3&=0  
\end{align}  
$$

From row 1:

$$
\begin{align}  
-v_1+v_2+v_3&=0\\  
-v_1+v_2&=0\\  
v_1&=v_2  
\end{align}  
$$

Let $v_2=t$:

$$
\mathbf{v}=t\begin{pmatrix}1\\1\\0\end{pmatrix},\ t\in\mathbb{R},\ t\neq0  
$$

## Case 2: $\lambda=2$

$$
\begin{align}  
(A-2I)\mathbf{v}&=0\\  
\begin{pmatrix}  
-2&1&1\\  
1&-2&1\\  
0&0&0  
\end{pmatrix}  
\begin{pmatrix}  
v_1\\v_2\\v_3  
\end{pmatrix}  
&=  
\begin{pmatrix}  
0\\0\\0  
\end{pmatrix}  
\end{align}  
$$

Augmented matrix:

$$
\left[  
\begin{array}{ccc|c}  
-2&1&1&0\\  
1&-2&1&0\\  
0&0&0&0  
\end{array}  
\right]  
$$

Gaussian elimination:

$$
\begin{align}  
R_2&\to 2R_2+R_1  
\end{align}  
$$

$$
\left[  
\begin{array}{ccc|c}  
-2&1&1&0\\  
0&-3&3&0\\  
0&0&0&0  
\end{array}  
\right]  
$$

Thus:

$$
\begin{align}  
-3v_2+3v_3&=0\\  
v_2&=v_3  
\end{align}  
$$

From row 1:

$$
\begin{align}  
-2v_1+v_2+v_3&=0\\  
2v_1&=v_2+v_3  
\end{align}  
$$

Let $v_3=t$. Since $v_2=v_3$, $v_2=t$:

$$
\begin{align}  
2v_1&=t+t\\  
v_1&=t  
\end{align}  
$$

Therefore:

$$
\mathbf{v}=t\begin{pmatrix}1\\1\\1\end{pmatrix},\ t\in\mathbb{R},\ t\neq0  
$$

## Case 3: $\lambda=-1$

$$
\begin{align}  
(A+I)\mathbf{v}&=0\\  
\begin{pmatrix}  
1&1&1\\  
1&1&1\\  
0&0&3  
\end{pmatrix}  
\begin{pmatrix}  
v_1\\v_2\\v_3  
\end{pmatrix}  
&=  
\begin{pmatrix}  
0\\0\\0  
\end{pmatrix}  
\end{align}  
$$

Augmented matrix:

$$
\left[  
\begin{array}{ccc|c}  
1&1&1&0\\  
1&1&1&0\\  
0&0&3&0  
\end{array}  
\right]  
$$

Gaussian elimination:

$$
\begin{align}  
R_2&\to R_2-R_1  
\end{align}  
$$

$$
\left[  
\begin{array}{ccc|c}  
1&1&1&0\\  
0&0&0&0\\  
0&0&3&0  
\end{array}  
\right]  
$$

$$
\begin{align}  
R_2&\leftrightarrow R_3  
\end{align}  
$$

$$
\left[  
\begin{array}{ccc|c}  
1&1&1&0\\  
0&0&3&0\\  
0&0&0&0  
\end{array}  
\right]  
$$

Thus:

$$
\begin{align}  
3v_3&=0\\  
v_3&=0  
\end{align}  
$$

From row 1:

$$
\begin{align}  
v_1+v_2+v_3&=0\\  
v_1+v_2&=0\\  
v_1&=-v_2  
\end{align}  
$$

Let $v_2=t$:

$$
\mathbf{v}=t\begin{pmatrix}-1\\1\\0\end{pmatrix},\ t\in\mathbb{R},\ t\neq0  
$$

## Final Answer

- $\lambda=1$, $\mathbf{v}=t\begin{pmatrix}1\\1\\0\end{pmatrix},\ t\neq0$
- $\lambda=2$, $\mathbf{v}=t\begin{pmatrix}1\\1\\1\end{pmatrix},\ t\neq0$
- $\lambda=-1$, $\mathbf{v}=t\begin{pmatrix}-1\\1\\0\end{pmatrix},\ t\neq0$
