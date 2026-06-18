Can be useful for [[Simplifying powers of matrices]].
See [[Question Type - Diagonalising matrices]]

> A matrix can only be diagonalised if the algebraic multiplicity is equal to the geometric multiplicity for every eigenvalue

> [!NOTE] Diagonalisation\
> If $V$ is the [[matrix]] whose columns are [[Eigenvector(s)]] of $A$, and $D$ is the diagonal matrix whose diagonal entries are the corresponding [[Eigenvalue(s)]]], then:
>
> $$
> AV=VD  
> $$
>
> Multiplying by $V^{-1}$ gives:
>
> $$
> \begin{align}  
> AVV^{-1}&=VDV^{-1}\\
> A&=VDV^{-1}  
> \end{align}  
> $$
>
> where:
>
> - $V$ = matrix whose columns are eigenvectors of $A$
>
> - $D$ = diagonal matrix containing the corresponding eigenvalues
>
> For an $n\times n$ matrix:
>
> - $A$ is diagonalizable if it has $n$ linearly independent eigenvectors
>
> - equivalently, the [[geometric multiplicity]] equals the [[algebraic multiplicity]] for every eigenvalue.

# Example

$$
A=\begin{pmatrix}
1&\frac12\\
1&\frac32
\end{pmatrix}
$$

Suppose $A$ has:

$$
\lambda_1=2,\quad \mathbf{v}_1=\begin{pmatrix}\frac12\\1\end{pmatrix}
$$

and

$$
\lambda_2=\frac12,\quad \mathbf{v}_2=\begin{pmatrix}-1\\1\end{pmatrix}
$$

Then:

$$
A\mathbf{v}_1=2\mathbf{v}_1,\qquad A\mathbf{v}_2=\frac12\mathbf{v}_2
$$

Construct a matrix $P$ whose columns are the eigenvectors:

$$
P=\begin{pmatrix}
\frac12&-1\\
1&1
\end{pmatrix}
$$

Construct a diagonal matrix $D$ whose diagonal entries are the corresponding eigenvalues in the same order:

$$
D=\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}
$$

Then:

$$
\begin{align}
AP
&=
A\begin{pmatrix}
\frac12&-1\\
1&1
\end{pmatrix}\\
&=
\begin{pmatrix}
A\mathbf{v}_1&A\mathbf{v}_2
\end{pmatrix}\\
&=
\begin{pmatrix}
2\mathbf{v}_1&\frac12\mathbf{v}_2
\end{pmatrix}\\
&=
\begin{pmatrix}
\frac12&-1\\
1&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}\\
&=PD
\end{align}
$$

Hence:

$$
AP=PD
$$

Multiplying both sides by $P^{-1}$:

$$
\begin{align}
APP^{-1}&=PDP^{-1}\\
A&=PDP^{-1}
\end{align}
$$

This is called the diagonalisation of $A$.
