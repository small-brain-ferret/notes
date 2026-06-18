# Example 1: Can diagonalise

Can the matrix

$$
A=\begin{pmatrix}
0&1&1\\
1&0&1\\
0&0&2
\end{pmatrix}
$$

be diagonalised? If so, write down its diagonalisation.

**Step 1: Check whether the matrix has enough linearly independent eigenvectors**

A matrix is diagonalisable if it has enough linearly independent eigenvectors (see [[linear dependency]]) to form the matrix $V$.

We have 3 distinct eigen values (see [[Question Type - Finding eigenvalues and eigenvectors]]),

$$
\lambda_1=1,\quad \lambda_2=2,\quad \lambda_3=-1
$$

with corresponding eigenvectors:

$$
\mathbf{v}_1=\begin{pmatrix}1\\1\\0\end{pmatrix},\quad
\mathbf{v}_2=\begin{pmatrix}1\\1\\1\end{pmatrix},\quad
\mathbf{v}_3=\begin{pmatrix}1\\-1\\0\end{pmatrix}
$$

Since there are three distinct eigenvalues, the eigenvectors are linearly independent. Therefore, $A$ is diagonalisable.

---

**Step 2: Construct $V$ using the eigenvectors as columns**

$$
V=\begin{pmatrix}
1&1&1\\
1&1&-1\\
0&1&0
\end{pmatrix}
$$

---

**Step 3: Construct $D$ using the corresponding eigenvalues in the same order**

Since the columns of $V$ are $\mathbf{v}_1,\mathbf{v}_2,\mathbf{v}_3$, the diagonal entries of $D$ must be $\lambda_1,\lambda_2,\lambda_3$ in the same order:

$$
D=\begin{pmatrix}
1&0&0\\
0&2&0\\
0&0&-1
\end{pmatrix}
$$

---

**Step 4: Write the diagonalisation**

$$
A=VDV^{-1}
$$

where

$$
V=\begin{pmatrix}
1&1&1\\
1&1&-1\\
0&1&0
\end{pmatrix},
\qquad
D=\begin{pmatrix}
1&0&0\\
0&2&0\\
0&0&-1
\end{pmatrix}
$$

# Example: can't diagonalise

Can the matrix

$$
A=\begin{pmatrix}
1&1&1\\
4&5&6\\
7&8&9
\end{pmatrix}
$$

be diagonalised? If so, write down its diagonalisation.

---

**Step 1: Check the eigenvalues and their multiplicities**

The matrix has eigenvalues:

$$
\lambda=0 \text{ (repeated)},\qquad \lambda=15
$$

For $\lambda=0$:

- algebraic multiplicity $=2$
- geometric multiplicity $=1$

---

**Step 2: Decide whether there are enough linearly independent eigenvectors**

A $3\times3$ matrix is diagonalisable if it has $3$ linearly independent eigenvectors.

Equivalently, for every eigenvalue:

$$
\text{geometric multiplicity}=\text{algebraic multiplicity}
$$

But for $\lambda=0$:

$$
\text{geometric multiplicity}=1<2=\text{algebraic multiplicity}
$$

So there are not enough linearly independent eigenvectors.

The matrix cannot be diagonalised.
